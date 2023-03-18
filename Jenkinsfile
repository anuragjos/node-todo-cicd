pipeline{
    agent any
    
    // // environment{
    //     DOCKERHUB_USERNAME = "anuragjoshi01"
    //     APP_NAME = "${node-app-cicd}"
    //     IMAGE_TAG = "${BUILD_NUMBER}"
    //     IMAGE_NAME = "${DOCKERHUB_USERNAME}"
    //     RIGSTRY_CREDS = 'dockerhub'
    // }

    stages{
        stage("Git Checkout"){
            steps{
                script{
                   git credentialsId: 'github',
                   url: 'https://github.com/anuragjos/node-todo-cicd.git',
                   branch: 'devops'
                }
            }
        }
        stage("Build Docker Image"){
            steps{
                script{
                    sh 'docker build -t anuragjoshi01/node-app-cide .'

                }
            }
        }
    }
}