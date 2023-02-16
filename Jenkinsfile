pipeline{
  agent any
  stages{
    stage('Build'){
      steps{
        sh 'g++ -c PES1UG20CS605.cpp'
        sh 'g++ -o PES1UG20CS605 PES1UG20CS605.cpp'
        echo 'Build Stage Successfull'
      }
    }
    stage('Test'){
      steps{
        sh './PES1UG20CS605'
        echo 'Test Stage Executed Successfull'
      }
    }
    stage('Deploy'){
      steps{
        echo 'Deploy Stage Successfull'
      }
    }
  }
  post{
    failure{
      echo 'Pipeline Failed'
    }
  }
}
    
