pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh 'g++ error.cpp -o error'
                 build job: 'PES1UG20CS307-1', wait: false
                 echo 'Build successful'
            }
        }

        stage('Test') {
            steps {
                sh 'cat pratham.cpp'
                echo 'Test successful'
            }
        }

        stage('Deploy') {
            steps {
               
                echo 'Deploy successful'
            }
        }
    }

    post {
        failure {
            
                echo 'Pipeline Failed'
          
        }
    }
}
