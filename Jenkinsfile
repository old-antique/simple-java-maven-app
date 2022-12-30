pipeline {
    stages {
        stage('Build') {
            steps {
                echo "1"
            }
        }
        stage('Test') {
            steps {
                echo "2"
            }
            post {
                always {
                    junit 'target/surefire-reports/*.xml'
                }
            }
        }
        stage('Deliver') {
            steps {
                echo "3"
            }
        }
    }
}
