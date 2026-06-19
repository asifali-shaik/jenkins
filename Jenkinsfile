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
                        exit 1
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
    post{
        always{
            echo 'happy !'
        }
        success{
            echo 'pipeline success !!'
        }
        failure{
            echo 'pipeline faliure !!!'
        }

    }
}  

    