pipeline {
    agent any

    stages {
        stage('Gmail'){
        steps{
            emailext body: "*${currentBuild.currentResult}:* Job Name: ${env.JOB_NAME} || Build Number: ${env.BUILD_NUMBER} || More information at: ${env.BUILD_URL}",
                subject: 'Declarative Pipeline Build Status',
                to: 'manjushreegs2022@gmail.com'
        }
    }
}

}

        
    


