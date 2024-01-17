pipeline {
agent {label 'dev'}
stages {
stage ('BUILD') {
  agent {label 'built-in'}
steps {
echo " hi"
}
}
stage ('DEPLOY') {
steps {
echo "how"
}
}
stage ('TEST') {
steps {
echo "why"
}
}
}
}
