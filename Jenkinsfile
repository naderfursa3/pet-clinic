pipeline {
    agent any
    // Stage begin here ...
    stages {
        //
        stage("Build") {
            steps {
                sh "mvn clean package"
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

