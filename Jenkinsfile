pipeline{
    agent any 
    environment {
        RELEASE = '22.0.0'
    }
    stages {
        stage ('build stage ') {
            environment {
                LOG_INFO = 'INFO'
            }
            steps {

                echo "building ${RELEASE} with ${LOG_INFO} "
            }
        }   

        stage ('testing') {
            steps {
            echo "Testing $RELEASE in progress"
            } 
        }
        stage ('Deploy') {
            input {
                message 'Deploy?'
                ok 'do it'
                parameters {
                    string(name: 'TAREGT_ENVIRONMENT', defaultValue: 'prod', description: 'deploying in prod')
                }

            }
            steps {
                echo "Deploying in $RELEASE TO environemnt $TARGET_ENVIRONMENT"
            }
        }
    }   
        post{
            always {
                echo "Print weither Deployment happened or not,success or fialure "
            }
        }    
}    
