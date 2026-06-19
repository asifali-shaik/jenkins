pipeline{
    agent {
        node{
            label 'roboshop'
        }
    }
    envrionment{
        name= "jenkins"
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
                        echo $name
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

    