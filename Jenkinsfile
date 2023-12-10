pipeline{
    
    agent any
    
    stages{
    
        stage('Echoing'){
    
            steps{
                //Basic directoy print and echo commands
                sh '''
                pwd
                echo "Hi Chris!"
                echo "Groovy Baby"
                echo "Inside shell block"
                '''
            }
    
        }
    
        stage('Run Script'){

            steps{
                //Basic directoy print and echo commands
                sh '''
                sh ./run.sh
                '''
            }

        }
    }
        post {
            always{
                archiveArtifacts '*.zip'
            }

        }
    
}