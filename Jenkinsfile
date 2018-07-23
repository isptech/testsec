
pipeline {
     agent {
        docker { image 'ubuntu' }
    }  
        stages {
        stage('Test for Secrets') {
            agent {
                docker {
                    image 'lvthillo/aws-cli'
                    args '-v $WORKSPACE:/project'
                    reuseNode true
                }
            }
            steps {
                sh 'echo "i am in the docker container" '
                sh 'aws --version'
            }
        }
    }
}
