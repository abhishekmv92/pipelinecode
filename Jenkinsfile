pipeline
{
  agent any
  
  stages{
    
    stage('compile stage'){
      steps{
        echo "compilation completed"
      }
    }
    
    stage('Testing'){
      steps{
        echo "Testing is successful"
      }
    }
    
    stage('Deploy'){
      steps{
        echo "Deployment is successful"
      }
    }
    
    
}
post{
    
    always{
      echo "It will execute always"
    }
    success{
       echo "only when it is sucess"
    }
    failure{
      echo "only when it is failure"
    }
    unstable{
      echo "only when it is unstable"
    }
    changed{
      echo "only when there is a change in pipeline"
    }
      
  }
}
