pipeline {
  agent any
   
  stages {
    stage('Build project') {
      steps {
        // Command 1
        sh 'echo "Building project...."'
        sh 'cd designs/leon3-xilinx-kcu105 && make vivado'
      }
    }   
  }
  post {
    failure {
      sh 'echo "Error failed to build"'
    }
  }
}
