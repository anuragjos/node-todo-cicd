pipeline{
    ageny any 
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
        // stage("Build and Test"){
        //     steps{
        //         script{

        //         }
        //     }
        // }
    }
}