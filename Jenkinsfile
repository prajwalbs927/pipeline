pipeline{
    agent none
    stages {
        stage ('Run parallel all stages') {
            parallel {
        stage ('Build'){
            agent {label 'dev'}
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
            agent {label 'built_in'}
            steps {
                echo "why"
            }
        }
            }
        }
    }
}
