pipeline{
    agent any

    stages{
        stage ('zip file'){
            step{
                sh ' zip -r ansible-${BUILD_ID}.zip * exclude Jenkinsfile '
            }


        }   
    }
}