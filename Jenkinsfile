pipeline{
    agent any

    stages{
        stage('zip the file'){
            steps{
                sh 'zip -r week7ansible-${BUILD_ID}.zip * --exclude Jenkinsfile'
            }
        }
        stage ('upload zip file to jfrog'){
            steps{
                sh 'curl -uadmin:AP4KPM9fdPBKovDyeDco7NnkZZV -T week7ansible-${BUILD_ID}.zip "http://18.207.1.230:8081/artifactory/myownprctice/"'
            }


        }

    }
}