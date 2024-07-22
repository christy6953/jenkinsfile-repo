pipeline {
    agent any

    environment {
        AWS_ACCESS_KEY_ID = credentials('aws-access-key-id')
        AWS_SECRET_ACCESS_KEY = credentials('aws-secret-access-key')
        AWS_DEFAULT_REGION = 'us-east-1'
    }

    stages {
        stage('AWS Demo') {
            steps {
                sh "aws s3 ls"
            }
        }

        stage ('show project name') {
            steps{
                echo "Project name is Vehicle-data"
            }
        }
    }
}