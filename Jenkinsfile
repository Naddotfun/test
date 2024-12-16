pipeline {
    agent any
    triggers {
        githubPush() // GitHub Push Event 트리거
    }

    stages {
        stage('Build') {
            steps {
                echo "🔧 Starting the build process at ${new Date()}"
                sh 'echo "Build process completed successfully!"'
            }
        }
        stage('Verify') {
            steps {
                echo "✅ Build verification complete!"
            }
        }
    }
    post {
        always {
            echo "🚀 Build completed, regardless of success or failure."
        }
    }
}
