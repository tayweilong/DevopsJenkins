pipeline {
  // where to execute (e.g. a node or executor)
  agent any
  // where the 'work' actually happens, consisting of stages and steps
  stages {
    stage("build") {
      steps {
       sh "mvn -version"
       sh "mvn clean install"
      }
    }
    stage("test") {
      steps {
        echo 'testing the app'
      }
    }
    stage("deploy") {
      steps {
        echo 'deploying the app'
      }
    }
  }
  post {
    always {
      // always start with a clean workspace
      cleanWs()
    
    }
  }
}
