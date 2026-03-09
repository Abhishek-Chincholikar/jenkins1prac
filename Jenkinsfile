pipeline{
  agent any

  stages{
    stage('Checkout){
      steps{
          git'https://github.com/Abhishek-Chincholikar/jenkins1prac.git'      
      }
    }
    stage('Publish'){
      steps{
        publishHTML([
          allowmissing:true,
          alwaysLinktoLastBuild:false,
          KeepAll:false,
          reportDir:'.',
          reportFiles:'index.html',
          reportName:'MY HTML PAGE'
          ])
      }
    }
  }
}
