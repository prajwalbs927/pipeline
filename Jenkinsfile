pipeline{
    agent none
    stages {
        stage ('RUN STAGES PARALLEL') {
        parallel {
            stage ('BUILD'){
                agent {label 'built-in'}
                steps {
                    echo "this is build stage"
                    sh 'sleep'
                }
            }
               stage ('TESt'){
                agent {label 'test1'}
                steps {
                    echo "this is test stage"
                    sh 'sleep'
                } 
               }
           stage ('DEPLOY'){
               agent {label 'node2'} 
               steps {
                    echo "this is deploy stage"
                    sh 'sleep'
                }
               }
        }
        }
    }
}
