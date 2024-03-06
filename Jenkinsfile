pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh 'g++ PES1UG21CS382.cpp -o temp'
                 build job: 'PES1UG21CS382', wait: false
                 echo 'Build by CS382 successful'
            }
        }

        stage('Test') {
            steps {
                sh 'cat PES1UG21CS382.cpp'
                echo 'Test by CS382 successful'
            }
        }

        stage('Deploy') {
            steps {
               
                 echo 'Deploy by CS382 successful'
            }
        }
    }

    post {
        failure {
            
                echo 'Pipeline Failed'
          
        }
    }
}
