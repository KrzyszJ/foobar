pipeline {
    agent any
    stages {
            stage('build') {
                steps {
                    sh '''
                        echo ('build')
                    '''
                }

            }
            stage('test') {
                    sh '''
                    ./run-tests
                    '''
            }

    }
}