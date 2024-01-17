pipeline{
    agent any
    stages {
        stage ('Run parallel all stages') {
            parallel {
        stage ('Build'){
            steps {
                echo "hello"
            }
        }
        stage ('test'){
            agent {label 'node2'}
steps {
    echo "how"
}
        }
        stage ('deploy') {
            agent {label 'built-in'}
            steps {
                echo "why"
            }
        }
            }
        }
    }
}
