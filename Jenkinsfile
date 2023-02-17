pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh 'g++ -o PES1UG20CS627-1 PES1UG20CS627.cpp'
                echo "Build Successful"
            }
        }
        stage('Test') {
            steps {
                sh './PES1UG20CS627-1'
            }
        }
    }
    post {
        always {
            echo 'Pipeline completed'
        }
        failure {
            echo 'Pipeline failed'
        }
    }
}
