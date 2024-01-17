pipeline{
    agent any
    stages {
        stage ('Run parallel all stages') {
            parallel {
        stage ('Build'){
            agent {label 'built-in'}
            steps {
                echo "hello"
                sh ''' /home/ubuntu/big2.sh 45 67
                sleep 5 '''
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
