pipeline {
    agent any

    stages {
        stage ('Docker Build') {
            steps {
                script {
                    sh 'sudodocker build -t fabio-tp-game .'
                    echo 'Build Image Completed'
                }    
            }
        }
   }
}
