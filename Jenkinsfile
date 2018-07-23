
node {
    def app
    stage('Clone the app') {
        checkout scm
    } 


    }
    
    stage("try to build in docker") {
        /* app = docker.build("isptech/gitscan:latest" ) */
        /* app = docker.run("isptech/gitscan:latest " ) */
        
        docker.image('isptech/gitscan').inside('-v $WORKSPACE:/codex') {
            sh 'ls /codex'
        }


    }
}
