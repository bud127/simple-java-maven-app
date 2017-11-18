pipeline {
  agent {
    docker {
      image 'simple-java-maven-app'
      args '-v /root/.m2:/root/.m2'
    }
    
  }
  stages {
    stage('Build') {
      steps {
        sh 'mvn -B -DskipTests clean package'
      }
    }
  }
}