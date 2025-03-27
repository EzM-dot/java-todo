pipeline{
    agent any
    tools {
        gradle "gradle"
    }
    stages{
        stage("Clone Repository"){
            steps{
                git branch:"master", url:"https://github.com/EzM-dot/java-todo.git"
            }
        }
        
        stage("Building code"){
            steps{
                sh "gradle build"
            }
            
        }
        stage("Testing code"){
            steps{
                sh "gradle test"
            }
        }
    }
}
