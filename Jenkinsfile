pipeline {
    agent any
    stages {
        stage('Clone Repository') {
            steps {
                // Clone the GitHub repository
                git branch: 'main', url: 'https://github.com/Sami-1166/ToCS_Project.git'
            }
        }
        stage('Deploy to Apache') {
            steps {
                // Transfer all relevant files to /var/www/html directory on Apache server
                sshPublisher(
                    publishers: [
                        sshPublisherDesc(
                            configName: 'apache-server', // Matches the SSH config name
                            transfers: [
                                sshTransfer(
                                    sourceFiles: '**/*.html, style.css', // Match all HTML and CSS files
                                    remoteDirectory: '/var/www/html/', // Target the correct directory
                                    removePrefix: '', // No prefix to remove
                                    cleanRemote: false // Keep existing files in the remote directory
                                )
                            ]
                        )
                    ]
                )
            }
        }

    }
 }
