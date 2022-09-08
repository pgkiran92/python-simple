@Library('SharedLibrary') _

node {
    stage('clone') { 
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
