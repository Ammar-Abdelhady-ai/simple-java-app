node {
    git branch: 'main', url: "https://github.com/Ammar-Abdelhady-ai/simple-java-app.git"
    
    stage(name: 'build') {
        try {
            sh 'echo "hello world"'
        } catch (Exception e) {
            sh 'echo "error"'
            throw e  // Re-throwing the error to fail the build
        }
    }

    stage(name: 'test') {
        if (env.BRANCH_NAME == "feat") {
            sh 'echo "feature branch"'
        } else {
            sh 'echo "feature not exist"'
        }
    }
}
