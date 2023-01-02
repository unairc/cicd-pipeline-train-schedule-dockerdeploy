pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                echo 'Running build automation'
                sh '/var/lib/jenkins/tools/hudson.plugins.gradle.GradleInstallation/GR/bin/gradle build'
                archiveArtifacts artifacts: 'dist/trainSchedule.zip'
            }
        }
    }
}
