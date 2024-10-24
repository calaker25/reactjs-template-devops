pipeline {
    agent any
    tools {
        nodejs 'node-latest'
    }

    stages {
        stage("Build and Deploy"){
            steps{
                echo "Using docker compose to build and deploy "
                sh """
                    docker compose up -d
                """
            }
        }

        stage("Add domain name"){
            steps{
                echo "Run shellscript to add domain "
            }
        }
    }
}