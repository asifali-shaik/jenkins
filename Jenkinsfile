pipeline{
    agent {
        node{
            label 'roboshop'
        }
    }
    stages{
        stage('build'){
            steps{
                script{
                    sh """
                        echo "build the image"
                    """
                }
            }
        }
        stage('test'){
            steps{
                script{
                    sh """
                        echo "testing the image"
                    """
                }
            }
        }
        stage('deploy'){
            steps{
                script{
                    sh """
                        echo "deploy the image"
                    """
                }
            }
        }
    }
}   // post build
    post{
        always{
            echo 'hello there pipeline is working!'
        }
    }