
pipeline {
    /*  agent {
        docker { image 'node' }
    }  */
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

/*
node {
	def app
	stage('Clone the app') {
		checkout scm
	} 

	stage("now doing another step") {
	echo "I am in my dir"
	}
	
	stage("try to build in docker") {
		/* app = docker.build("isptech/gitscan:latest" ) */
		/* app = docker.run("isptech/gitscan:latest " ) */

	}
}
*/

