pipeline {
agent none
  environment {
    name = 'prajwal'
  }
  stages {
    stage ('RUN Parallel') {
    parallel {
    stage ('BUILD') {
      agent {label 'node2'}
  steps {
    echo "This is build stage $name "
    sh 'sleep 5'
    echo $name 
    exit 0
  }
}
    stage ('TEST') {
       agent {label 'built-in'}
  steps {
    echo "This is test stage"
    sh 'sleep 5'
} 
    }
    }
}
    stage ('DEPLOY parallel') {
      parallel {
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
