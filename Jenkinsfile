pipeline {
    agent none
    environment {
        NODE_VER = '8.1.0'
    }
    stages {
        stage('Beginning') {
            environment {
                NEW_VAR = 'Boo'
            }
            agent any
            steps {
                echo 'Hello World'
                echo "${env.NEW_VAR}"
                echo env.NODE_VER
            }
        }
        stage('Jakes stage'){
            agent any
            steps {
                bat 'nslookup jjaobson20163.mainman.dcs'
            }
        }
    }
}