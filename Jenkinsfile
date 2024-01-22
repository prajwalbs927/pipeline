pipeline{
    agent none
    stages {
        stage ('RUN STAGES PARALLEL') {
        parallel {
            stage ('BUILD'){
                agent {label 'built-in'}
                steps {
                    echo "this is build stage"
        
                    
                }
            }
               stage ('TEST'){
                agent {label 'test1'}
                steps {
                    echo "this is test stage"
                    
                } 
               }
           stage ('DEPLOY'){
               agent {label 'node2'} 
               steps {
                    echo "this is deploy stage"
                    
                }
               }
        }
        }
    }
}
