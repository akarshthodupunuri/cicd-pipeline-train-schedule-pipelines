pipeline {
    agent any
    stages{
        stage('build') { 
            steps {
            echo "building the zip arhive and running tests"
            sh './gradlew build --no-daemon'
            archiveArtifacts 'dist/trainSchedule.zip'
            }
        }
    }
}
