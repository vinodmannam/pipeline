def workspace;
node
{
    stage('checkout')
    {
        checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[credentialsId: 'e5574485-5931-4e7a-8f9f-d47e883d8eeb', url: 'https://github.com/vinodmannam/pipeline.git']]])
        workspace = pwd()
    }
    stage('Static Code Analysis')
    {
        echo "Static Code Analysis"
    }
    stage('Build')
    {
        echo "Build the Code"
    }
    stage('Unit Testing')
    {
        echo "Unit Testing"
    }
    stage('Delivery')
    {
        echo "deliver the code"
    }
}
