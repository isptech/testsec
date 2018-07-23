node {
	def app
	stage('Clone the app') {
		checkout scm
	} 

	stage("now doing another step") {
	echo "going away"
	}
	
	stage("try to build in docker") {
		/* app = docker.build("isptech/gitscan:latest" ) */
		/* app = docker.run("isptech/gitscan:latest " ) */
	}
}

