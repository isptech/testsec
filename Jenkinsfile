
node {
    def app
    stage('Clone the app') {
        checkout scm
    } 


    stage("try to build in docker") {
        /* app = docker.build("isptech/gitscan:latest" ) */
        /* app = docker.run("isptech/gitscan:latest " ) */
        
        docker.image('isptech/gitsecret1:latest').inside('-v $WORKSPACE:/codes -w /codes') {
            /* sh 'bash /src/run.sh' */ 
        }

    }
}

/*
if [ $? -eq 0 ]; then
        echo "git secrets --scan OK"
    else
    echo "git secrets --scan FAIL"    
    */  