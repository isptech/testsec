/*
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
*/

node {
    def app
    stage('Clone the app') {
        checkout scm
    } 

    stage("now doing another step") {
                   /* docker {
                    image 'lvthillo/aws-cli'
                    args '-v $WORKSPACE:/project'
                    reuseNode true
                } */ 
            


    }
    
    stage("try to build in docker") {
        /* app = docker.build("isptech/gitscan:latest" ) */
        /* app = docker.run("isptech/gitscan:latest " ) */

    }
}
