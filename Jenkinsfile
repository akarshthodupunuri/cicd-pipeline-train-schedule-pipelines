pipeline {
    agents any
    stages {
        stage('build') {
            steps {
                echo "Running build automation and creating zip archive"
                sh './gradlew build --no-daemon'
                archiveArtifacts 'dist/trainSchedule.zip'
            }
        }
    }
}
