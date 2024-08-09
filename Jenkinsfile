pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                script {
                    // Install dependencies
                    sh 'npm install'
                }
            }
        }
        stage('Deploy') {
            steps {
                script {
                    // Deploy to Render
                    sh 'npm start'
                }
            }
        }
    }
    post {
        success {
            script {
                // Notify on Slack
                slackSend (channel: '#Brian_IP1', 
                            message: "Build ${env.BUILD_ID} successfully deployed to Render: ${env.RENDER_URL}")
            }
        }
    }
}
