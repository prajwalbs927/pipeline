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
steps {
    echo "how"
}
        }
        stage ('deploy') {
            steps {
                echo "why"
            }
        }
            }
        }
    }
}
