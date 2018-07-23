
node {
    def app
    stage('Clone the app') {
        checkout scm
    } 


    }
    
    stage("try to build in docker") {
        /* app = docker.build("isptech/gitscan:latest" ) */
        /* app = docker.run("isptech/gitscan:latest " ) */
        -v $WORKSPACE:/output
        docker.image('isptech/gitscan').inside("-v $WORKSPACE:/codex) {
            /*
             * Run some tests which require MySQL, and assume that it is
             * available on the host name `db`
             */
            sh 'ls /codex'
        }


    }
}
