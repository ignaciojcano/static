pipeline {
    agent any
    stages {
        stage('Upload to AWS') {
            steps {
                withAWS(region:'us-west-2', credentials:'aws-static') {
                    s3Upload(file:'index.html', bucket:'udacity-p3-bucket-nacho', path:'./index.html')
                }
            }
        }
    }
}