pipeline{
    agent any
    environment {
        DEMO = '1'
        JOB_NAME = 'MY job name'
    }
    stages{
        stage("build"){
            steps {
                echo " build number $DEMO"
            }

        }
        stage("job name"){
            steps {
                sh '''
                echo "my job name is $JOB_NAME" 
                
                '''
            }
        }
    }
}
    
