pipeline {
    agent any

    stages {
        stage('Cloning Git') {
            steps {
                /* Let's make sure we have the repository cloned to our workspace */
                checkout scm
            }
        }
        stage('SAST') {
            steps {
                sh 'echo SAST stage'
            }
        }
        stage('Build-and-Tag') {
            steps {
                /* This builds the actual image; synonymous to
                 * docker build on the command line */
                sh 'echo Build and Tag'
            }
        }
        stage('Post-to-dockerhub') {
            steps {
                sh 'echo post to dockerhub repo'
            }
        }
        stage('SECURITY-IMAGE-SCANNER') {
            steps {
                sh 'echo scan image for security'
            }
        }
    }
}

