pipeline {
    agent none
    stages {
        stage('Beginning') {
            agent any
            steps {
                echo 'Hello World'
            }
        }
        stage('Jakes stage'){
            agent any
            steps {
                sh 'host -t TXT jjaobson20163.mainman.dcs'
            }
        }
    }
}