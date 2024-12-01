node{
    git branch: 'main', url: "https://github.com/Ammar-Abdelhady-ai/simple-java-app.git"
    stage(name: 'build'){
        try{
            sh'echo "hello world"'
        }
        cache(Exception e)
            sh'echo "error"'
            throw e
    }

    stage(name: 'test'){
        if (env.BRANCH_NAME == "feat"){
            sh'echo "feature branch"'
        }
        
        else{
            sh'echo "feature not exist"'
        }
    }
}