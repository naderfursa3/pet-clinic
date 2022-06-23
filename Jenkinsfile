pipeline {
    agent any

    
    stages {
        //
        stage("Build") {
            steps {
                sh "./mvnw clean package"
            }
        }
        //
    
        stage("Save Artifact") {
            steps {
                archiveArtifacts artifacts: 'target/*.jar', followSymlinks: false
            }
        }
    }
}

