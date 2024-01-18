pipeline {
agent none
  stages {
    stage ('DEPLOY parallel') {
      parallel {
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
    
      stage ('Deploy') {
      agent {label 'test1'}
  steps {
    echo "This is deploy stage"
    sh 'sleep 5'
  }
    }
      }
    }
}
}
