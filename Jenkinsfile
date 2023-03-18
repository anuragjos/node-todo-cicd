pipeline{
    ageny any 
    stages{
        stage("Git Checkout"){
            steps{
                script{
                    git branch: 'devops', url: 'https://github.com/anuragjos/node-todo-cicd.git'
                }
            }
        }
    }
}