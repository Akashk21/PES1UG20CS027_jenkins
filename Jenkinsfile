pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh 'g++ srn.cpp'
                echo "Build Successful!"
            }
        }
      stage('Test') {
        steps {
          sh './a.out'
          echo "Yay Successful!"
        }
      }
      stage('Deploy') {
          steps {
        echo "Deploy"
          }
      }
    }
    post {
        failure {
            echo "Pipeline failed!"
        }
    }
}
