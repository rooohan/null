pipeline {
  agent any
  stages {
    stage('step1') {
      steps {
        echo 'start'
		env.imageTag = sh (script: 'git rev-parse --short HEAD ${GIT_COMMIT}', returnStdout: true).trim()
      }
    }

  }
  environment {
    nohup = 'G:\\Import\\Git\\usr\\bin'
    SHELL = 'G:\\Import\\Git\\bin\\sh.exe'
    PATH = 'G:\\APP\\Matlab\\bin\\win64;G:\\Import\\Git\\bin\\sh.exe'
  }
}