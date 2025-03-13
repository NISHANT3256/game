pipeline{
    tools{
        jdk 'myjdk'
        maven 'mymvn'
    }
    agent none
    stages{
        stage('Checkout'){
            agent any
            steps{
                git 'https://github.com/NISHANT3256/game.git'
            }
        }
        stage('Compile'){
            agent any
            steps{
                sh 'mvn compile'
                
            }
        }
        stage('Package'){
            agent any
            steps{
                sh 'mvn package'
                
            }
        }


    }
}
