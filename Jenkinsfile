pipeline{
    agent any
    environment{
        BUILD_VERSION="1.0"
    }
    stages{
        stage('Clone Repository'){
            steps{
                script{
                    def workspace=env.WORKSPACE
                    def cloneJSP="${workspace}\\cloneJSP"
                    if(fileExists(cloneJSP)){
                        bat "rmdir /S /Q \"${cloneJSP}\""
                        echo "Removed existing Repo folder."
                    }
                    bat "mkdir cloneJSP"
                    bat "cd ${workspace}\\cloneJSP"
                    //git branch: 'master', credentialsId: 'JSPCookiesToken', url:'https://github.com/poudwalsamruddhi-alt/jenkins.git'

                    bat "git clone https://github.com/poudwalsamruddhi-alt/jenkins.git \"${cloneJSP}\""
                }
            }
