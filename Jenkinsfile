pipeline{
    agent any
    stages{
        stage('Build'){
            steps{
                sh 'g++ -c PES1UG20CS605-1.cpp'
                sh 'g++ -o PES1UG20CS605 PES1UG20CS605-1.cpp'
                echo 'BUILD IS SUCCESSFULL'
            }
        }
        stage('Test'){
            steps{
                sh './PES1UG20CS605'
                echo 'TEST EXECUTED SUCCESSFULLY'
            }
        }
        stage('Deploys'){
            steps{
                echo 'DEPLOY SUCCESSFULL'
            }
        }
    }
    post{
        failure{
            echo 'PIPELINE FAILED'
        }
    }
}
