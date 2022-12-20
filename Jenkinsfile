pipeline {
    agent any

    stages {
        stage('checkout') {
            steps {
                git 'https://github.com/opstree/spring3hibernate.git'
            }
        }
        stage('codestability') {
            steps {
                echo 'code stability'
            }
        }    
        stage('code_analysis') {
            steps {
                echo 'code analysis'
            }
        }
        stage('code_coverage') {
            steps {
                echo 'code coverage'
            }
        }
        stage('generating_report') {
            steps {
                echo 'generating report'
            }
        }
        stage('publish_artifacts') {
            steps {
                echo 'publish artifacts'
            }
        }
        stage('email_notification') {
            steps {
                echo 'email notification'
            }
        }
    }
}
