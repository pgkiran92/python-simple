@Library('SharedLibrary') _

node {
    stage('checkout') { 
        checkout scm        
    }
    stage('Initialize'){
        DockerInitialize()
    }
    stage('build') {
        DockerBuild("premkiran","docker_images")
    }
    stage('logout')
    {
        DockerLogout()
    }
}
