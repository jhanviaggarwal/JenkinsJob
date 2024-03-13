pipeline {
    agent any
    
    stages {
        stage('Build') {
            steps {
                // Your build commands here
                echo 'Build app'
            }
        }
        stage('Test') {
            steps {
                // Your test commands here
               echo 'test app' // Example Maven test command
            }
        }
        stage('Deploy') {
            steps {
                // Your deployment commands here
                echo 'deploy app'
            }
        }
        post {
            always {
                // Your post-deployment actions here
               mail bcc: '', body: 'Successfull', cc: '', from: '', replyTo: '', subject: 'Jenkins Pipeline Status', to: 'jhanviaggarwal1610@gmail.com'
            }
        }
    }
}
