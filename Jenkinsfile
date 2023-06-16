pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                echo 'Build stage'
            }
        }
        stage('Test') {
            steps {
                echo 'Test stage'
                sh '''
                "chmod +x ./run-tests.sh
                '''
                sh '''
                    ./run-tests.sh
                    '''
            }
        }
    }
        post { 
            always { 
                echo 'I will always say Hello again!'
        }
    }
}