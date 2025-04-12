pipeline{
    agent any;
    stages{
        stage("clone"){
            steps{
                git credentialsId: '27c48c0c-bf2c-4ac2-9607-6dd66739b413', url: 'https://github.com/Rohan007-rishi/gitpct_2.git'
            }
            post{
                success{
                    echo "Successfully cloned "
                }
                failure{
                    echo "Failed to clone"
                }
            }
        }
    }
    post{
        success{
            echo "pipeline executed successfully"
        }
        failure{
            echo "pipeline execution failed"
        }
    }
}