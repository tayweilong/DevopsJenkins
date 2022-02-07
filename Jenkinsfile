pipeline {
  // where to execute (e.g. a node or executor)
  agent any
  // where the 'work' actually happens, consisting of stages and steps
  stages {
    stage("build") {
      steps {
        echo 'building the app part 2'
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
}
