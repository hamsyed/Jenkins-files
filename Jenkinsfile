pipeline{
    agent any
    environment {
        DEMO = '1'
    }
    stages{
        stage("build"){
            steps {
                echo " build number $DEMO"
            }

        }
        stage("job name"){
            steps {
                sh ' echo "my job name is $JOB_NAME "'
            }
        }
    }
}
    
