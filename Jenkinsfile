pipeline{
  agent any
  stages{
    stage('Build'){
    steps{
      sh 'g++ testfile.cpp -o PES1UG20CS397'
      echo 'Build Successful'
    }
  }
  stage('Test'){
    steps{
      sh './PES1UG20CS397'
    }
  }
  stage('Deploy'){
    steps{
      echo 'Deployment Success'
    }
  }
  }
  post{
    failure{
      echo 'Build Failed!'
    }
  }
  
}
