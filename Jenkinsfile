pipeline {
agent none
  stages {
    stage ('BUILD') {
      agent {label 'node2'}
  steps {
    echo "This is build stage"
    sh 'sleep 5'
  }
}
    stage ('TEST') {
       agent {label 'built-in'}
  steps {
    echo "This is test stage"
    sh 'sleep 5'
} 
}
    stage ('DEPLOY') {
      agent {label 'node2'}
  steps {
    echo "This is deploy stage"
    sh 'sleep 5'
  }
    }
  }
}
