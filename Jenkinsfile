pipeline {
agent none
stages {
  stage {
    prarallel {
stage ('BUILD') {
  agent {label 'built-in'}
steps {
echo " hi"
}
}
stage ('DEPLOY') {
  agent {label 'test1'}
steps {
echo "how"
}
}
    }
  }
stage ('TEST') {
  agent {label 'node2'}
steps {
echo "why"
}
}
}
}
