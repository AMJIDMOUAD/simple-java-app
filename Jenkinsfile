node {

    git branch: 'declarativepip', url: 'https://github.com/AMJIDMOUAD/simple-java-app.git'

    stage('Build') {
        sh 'echo "Building..."'
    }
    stage('Test') {
        sh 'echo "Testing..."'
    }
    stage('Deploy') {
       try {
            if (env.BRANCH_NAME == 'declarativepip') {
                sh 'echo "Deploying to production..."'
            } 
        } catch (Exception e) {
            echo "Deployment failed: ${e.message}"
        }
    }
}