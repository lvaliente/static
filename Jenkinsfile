pipeline {
    agent any
    stages {
        stage('Lint HTML') {
            steps {
                sh 'tidy -q -e index.html'
            }
        }
        stage('Run Hello World without load to AWS') {
            steps {
		    sh 'echo "Hello World with AWS creds"'
            }
        }
    }
}
