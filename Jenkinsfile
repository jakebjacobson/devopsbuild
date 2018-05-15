pipeline {
    agent none
    environment {
        NODE_VER = '8.1.0'
    }
    stages {
        stage('Beginning') {
            environment {
                DEPLOY_VERSION = 'stage'
            }
            agent any
            steps {
                echo 'Hello World'
                echo "${env.DEPLOY_VERSION}"
                echo env.NODE_VER
            }
        }
        stage('Jakes stage'){
            agent any
            stage('Beginning') {
                environment {
                    DEPLOY_VERSION = 'production'
                }
            steps {
                bat 'nslookup jjaobson20163.mainman.dcs'
                echo "${env.DEPLOY_VERSION}"
            }
        }
    }
}