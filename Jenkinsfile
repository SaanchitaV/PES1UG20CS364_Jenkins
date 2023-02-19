pipeline{
  agent any
  
  stages{
    stage('Build'){
      steps {
        sh 'g++ -o PES1UG20CS364-1 newfile.cpp'
      }
    }
    
    stage('Test'){
      steps {
        sh './PES1UG20CS364-1111'
      }
    }
    
    stage('Deploy') {
      steps{
        echo 'Deployment Successful'
      }
    }
  }
  
  post{
    always{
      echo 'Pipeline Finished'
    }
    
    failure{
      echo 'Pipeline Failed'
    }
  }
}
