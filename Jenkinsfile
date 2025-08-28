pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo "Building on all branches..."
                sh "echo Simulating Maven build process"
            }
        }

        stage('Test') {
            steps {
                echo "Running tests on all branches..."
                sh "echo Simulating Maven test process"
            }
        }

        stage('Deploy') {
            when {
                branch 'main'
            }
            steps {
                echo "Deploying only on main branch..."
                sh "echo Deploying build number ${env.BUILD_NUMBER} to Production"
            }
        }
    }
}
