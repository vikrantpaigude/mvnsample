pipeline{
    agent {label 'slave01'}
    stages{
        stage('clone01'){
            steps{
                git 'https://github.com/vikrantpaigude/mvnsample.git'
            }
        }
        stage('build02'){
            steps{
                sh 'mvn clean package'
            }
        }
        stage('archieve03'){
            steps{
                sh 'sudo cp /home/ubuntu/slave01/workspace/tp/target/*.war /home/vikrant'
            }
        }
    }
}
