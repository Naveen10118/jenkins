pipeline {
    agent {
        node {
            label 'docker-agent-python'
        }
    }
        stages {
            stage('Build') {
                steps { 
                    echo "Building.."
                    sh '''
                    echo "doing build stuff..."
                    '''
                }
            }
            stage('Test') {
                steps { 
                    echo "Testing.."
                    sh '''
                    echo "doing test stuff..."
                    '''
                }
            }
            stage('Deliver') {
                steps { 
                    echo "Delivering.."
                    sh '''
                    echo "doing deliver stuff..."
                    ''' 
                }
            }
        }
        
        post { 
            success { 
                echo 'Pipeline executed successfully!' 
            } 
            failure { 
                echo 'Pipeline execution failed!' 
        }
    }
    
}
