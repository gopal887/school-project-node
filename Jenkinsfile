pipeline{
    agent {label 'SCHOOL-T'}
    stages{
        stage('continuous-download'){
            steps{
                git 'https://github.com/balla26/school-project-node.git'
                branch 'main'
            }
        }
        stage('continuous-build'){
            steps{
                sh 'sudo apt install npm git -y'
                sh 'npm start'
            }
        }
    }
}