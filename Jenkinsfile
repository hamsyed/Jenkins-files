pipeline{
    agent any 
    environment {
        RELEASE = '20.0.1'
    }
    stages {
        stage ('build') {
            agent any 
            environment {
                LOG_LEVEL = 'INFO'
            }
            steps {
                echo "Building release $RELEASE with $LOG_LEVEL"
            }

        }
        stage ('TEST') {
            steps {
                echo "testing Release $RELEASE with $LOG_LEVEL"
            }
        }
    }
