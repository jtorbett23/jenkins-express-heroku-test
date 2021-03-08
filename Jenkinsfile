pipeline {

    agent any

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
}