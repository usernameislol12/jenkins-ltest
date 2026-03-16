pipeline{
  agent any
  stages{
    stage('Clone'){
      steps{
        git url: "https://github.com/usernameislol12/jenkins-ltest.git",branch:"main"
      }
    }
    stage('Run Script'){
      steps{
        sh 'chmod +x script.sh'
        sh './script.sh'
      }
    }
    stage('Check python'){
      steps{
        sh 'python3 --version'
      }
    }
    stage('Run Pyton File'){
      steps{
        sh 'python3 app.py'
      }
    }
  }
}
