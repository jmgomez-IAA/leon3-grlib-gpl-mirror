pipeline {
  agent any
   
  stages {
    stage('Build project') {
      steps {
        // Command 1
        echo "Building project...."
        cd designs/leon3-xilinx-kcu105
        make vivado        
      }
    }   
  }
  post {
    failure {
      echo "Error failed to build"
    }
  }
}
