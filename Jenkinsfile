pipeline {
    agent any 
     stages {
        stage('stage01-This is my first stage') {
            steps {
                sh 'cal'
            }
        } 
        stage('stage02-This is my second stage') {
            steps {
                sh 'pwdd'
            }
        }
        stage('stage03-This is my Third stage') {
            steps {
                sh 'echo $USER'
            }
        }
     }
    post {
        always {
            echo 'Yours Jenkins has been run !'
        }
        failure {
            echo 'Your Jenkins has been failed, please resolve it as soon as possible !'
        }
        success {
            echo 'Your Jenkins has been run successfully !'
        }
    }
}
