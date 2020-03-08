def workspace
node
{
    stage('checkout')
    {
        checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[credentialsId: 'fd034e46-ef67-4bf5-9e35-774ba5aa82d1', url: 'https://github.com/nagabrahmatejach/repo2.git']]])
        workspace =pwd()
    }
    stage ('static code analysis')
    {
        echo "static code analysis"
    }
    stage ('Build')
    {
        echo "Build the code"
    }
    stage ('Unit Testing')
    {
        echo "Unit Testing the code"
    }
    stage ('Delivery the code')
    {
        echo "Delivery the code"
    }
}
