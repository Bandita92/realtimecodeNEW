pipeline{
    agent any 
    stages{
        stage ("git checkout"){
            steps{
                git credentialsId: 'mygithub', url: 'https://github.com/Bandita92/realtimecodeNEW.git'
                echo "git checkout"
            }
        }
        stage ("compile"){
            steps{
                sh 'mvn compile'
                echo "compile job done"
            }
            
        }
        stage ("test"){
            steps{
                sh 'mvn test'
                echo "test job done"
            }
            
        }
        stage ("package"){
            steps{
                sh 'mvn package'
                echo "package job doen"
            }
            
        }
    }
}
