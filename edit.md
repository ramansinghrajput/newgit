pipeline {
    agent any
    parameters {
        string(name: 'name')
    }
    stages {
        stage('Hello') {
            steps {
                echo 'Hello world'
            }
        }
        stage('string') {
            steps {
                echo "Hello $name"
            }
        }
    stage('Example') {
            input {
                message "Should we continue?"
                ok "Yes, we should."
                submitter "alice,bob"
                parameters {
                    string(name: 'PERSON', defaultValue: 'Mr Jenkins', description: 'Who should I say hello to?')
                }
            }
            steps {
                echo "Hello, ${PERSON}, nice to meet you."
            }
        }      
    }
}


