pipeline{
agent none
    stages {
stage ('Run parallel build and test') {
    parallel {
        stage ('BUILD') {
agent {label 'built-in'}
            steps {
                echo "this is build stage"
        }
    }
        stage ('DEPLOY') {
            agent {label 'test1'} 
            steps {
                echo "this is deploy stage"
            }
        }
    }

}
stage ('TEST') {
    agent {label 'node2'}
    steps {
        echo "this is test stage"
    }
}
    }
}
