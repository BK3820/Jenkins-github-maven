pipeline {
    agent any

    tools {
        // Install the Maven version configured as "M3" and add it to the path.
        maven "M399"
    }
    
    stages{
        stage('First stage'){
            steps{
                sh "echo PRINTING MAVEN VERSION"
                sh "mvn -version"
            }
        }
        
        stage('MVN CLEAN'){
            steps{
                //git branch: 'main', url: 'https://github.com/BK3820/Jenkins-github-maven.git'
                
                sh "mvn clean package -DskipTests=true"
            }

        }
        
        stage('TEST'){
            steps{
                sh "mvn test"
            }
        }
    }


    }

