pipeline
{
  agent any
  
  stages{
    
     stage('Checkout from git'){
      steps{
        echo "compilation completed"
        git 'https://github.com/abhishekmv92/pipelinecode.git'
        
      }
    }
    
    stage('Build from git'){
      steps{
        echo "compilation completed"
        bat label: '', script: 'Build.bat'
        
      }
    }
    
    stage('compile stage'){
      steps{
        echo "compilation completed"
        bat label: '', script: 'compiled.bat'
      }
    }
    
    stage('Testing'){
      steps{
        echo "Testing is successful"
        bat label: '', script: 'test.bat'
      }
    }
    
    stage('Deploy'){
      steps{
        echo "Deployment is successful"
        bat label: '', script: 'deploy.bat'
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
