pipeline {
agent {
  label 'built-in'
}
  stages {
    stage ('BUILD') {
  steps {
    echo "This is build stage"
    sh 'sleep 5'
  }
}
    stage ('TEST') {
  steps {
    echo "This is test stage"
    sh 'sleep 5'
} 
}
    stage ('DEPLOY') {
  steps {
    echo "This is deploy stage"
    sh 'sleep 5'
  }
    }
  }
}
