pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh 'g++ -o filename filename.cpp'
                build job: "PES1UG20CS627-1", wait: true
                echo 'building PES1UG20CS627-1 job successful'
                echo 'build stage successful'
            }
        }
        stage('Test') {
            steps {
                sh './filename'
                echo 'test stage successful'
            }
        }
        stage('Deploy') {
            steps {
                sh 'echo "Deploying "'
                echo 'deployment successful'
            }
        }
    }
    post {
        failure {
          echo 'pipeline failed'
                }
            
        
    }
}
   
