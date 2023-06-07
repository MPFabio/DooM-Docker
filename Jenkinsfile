pipeline {
    agent any

    stages {
        stage ('Docker Build') {
            steps {
                script {
                    sh 'sudo docker build -t fabio-tp-game .'
                    echo 'Build Image Completed'
                }    
            }
        }

        stage ('Docker Tag') {
            steps {
                script {
                    sh 'docker tag fabio-tp-game fabiomp/fabio-tp-game'
                }
            }
        }

        stage('Docker Login') {
            steps {
                script {
                    sh 'docker login -u fabiomp -p Aucunmdp69' 
                }    
            }
        }

        stage ('Docker Push') {
            steps {
                script {
                    sh 'docker push fabiomp/fabio-tp-game'        
                }    
            }
        }    
    }
}
