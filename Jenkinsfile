pipeline {

    agent {
        docker {
            image 'node:lts-alpine' 
            args '-p 3000:3000' 
        }
    }

    stages {

        stage("build")
        {
            steps {
                echo 'building the applciation...'
                sh 'npm install'
            }
        }

        stage("test")
        {
            steps {
                echo 'testing the application...'
            }
        }

        stage("deploy")
        {
            steps {
                echo 'deploying the application...'
            }
        }
    }

    post {
        success {
            echo 'build was successful'
        }

        failure {
            echo 'build has failed'
        }
    }
}