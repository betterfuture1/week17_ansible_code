pipeline{
    agent any

    stages{
        stage('zip the file'){
            steps{
                sh 'zip -r week7ansible-${BUILD_ID}.zip * --exclude Jenkinsfile'
            }
        }
    }
}