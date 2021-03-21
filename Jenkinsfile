pipeline {
    agent docker {image 'python'}
    stages {
        stage('Run Tests') {
            parallel {
                stage('Test On Windows') {
                   
                    steps {
                        sh 'python3 -m pytest'
                    }                    
                }
                stage('Test On Linux') {
                    
                    steps {
                        sh 'python3 -m pytest'
                    }
                }
            }
        }
    }
}
