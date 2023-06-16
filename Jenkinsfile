pipeline {
    agent {
        dockerfile {
            filename 'Dockerfile'
        }
    }
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
                    ./run-tests.sh
                    '''
                sh '''
                    curl -s https://example.org/ | grep -F '<title>'
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