pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                // This checks out the code from the repository.
                git(url: 'https://github.com/GidSamina/MySoftware.git', branch: 'main')
            }
        }
        stage('Run Script') {
            steps {
                    echo "Running NewButton.py and NewScreen.py on main branch..."
                    bat  'python NewButton.py', 'python NewScreen.py'
                }
            }
        }

}