node{
    stage("Checkout"){
     git"https://github.com/Michaell99/practice1.git"
    }
    stage("Build"){
        bat "docker build -t practiceapp . "
    }
    stage("Test"){
        bat "python hello-world.py"
    }
    stage("Push"){
        bat "docker tag practiceapp michaelliav/practiceapp:v1"
        bat "docker push michaelliav/practiceapp:v1"
    }
}

