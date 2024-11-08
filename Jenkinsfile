//This is Jenkins file for pipeline
//Add proper structure in this

//Pipeline->Stages->stage

//Jenkinsfile (This name should be same as in Jenkins)
pipeline{
    agent any
    stages{
        // Clone Repo
        stage('Clone repo')
        {
            steps{
                git branch:'main', url:'https://github.com/Maulavi-azreen/Jenkins.git'
            }
        }

        // Install Dependencies
        stage('Install Dependencies'){
            steps{
                sh 'npm install'
            }
        }

        // Testing App
        // stage('Testing my application'){
        //     steps{
        //         sh 'npm test'
        //     }
        // }

        // start the application
        stage('Start the application'){
            input{
                message 'Do you really want to start'
                ok "Click on ok"
                submitter "Azreen"
            }
            steps{
                sh 'npm start'
            }
        }
    }
}