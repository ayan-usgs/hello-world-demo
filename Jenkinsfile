@Library(value='DemoLibrary', changelog=false) _

pipeline {
    agent {
        node {
            label 'project:any'
        }
    }
    triggers {
        pollSCM('H/5 * * * *')
    }
    stages {
        stage('build stage') {
            steps {
                demoPipeline()
            }
        }
    }
}
