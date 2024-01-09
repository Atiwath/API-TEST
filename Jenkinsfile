pipeline {
    agent any
    
    stages {
        stage('Install Python 3.10') {
            steps {
                script {
                    // Adjust these commands based on your operating system
                    def installCmd
                    if (isUnix()) {
                        installCmd = """
                            sudo apt update
                            sudo apt install -y python3.10
                        """
                    } else {
                        // Add Windows installation command if needed
                        // Example for Windows:
                        // installCmd = "choco install python3.10 -y"
                    }

                    sh installCmd
                }
            }
        }

        stage('Verify Python Installation') {
            steps {
                script {
                    sh 'python3.10 --version'
                }
            }
        }

        // Add more stages as needed for your Jenkins pipeline
    }
}
