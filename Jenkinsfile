node{
    git branch: "master", url: 'https://github.com/MahmoudMohamedRashad/remote-demo.git'
    stage('build'){
        try{
            sh'echo "your build stage sucess!"'
        } 
        catch(Exception error){
            sh'echo "build stage failed"'
        }
    stage('testing'){
        if(env.BRANCH_NAME == "main"){
            sh'echo "hello from main! your test success"'
        }
        else{
            sh'echo "branch error"'
        }
    }
    }
 }
