def workspace
node
{
    stage('checkout')
    {
        checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[credentialsId: '8e642e89-5243-4397-b76c-034378b02ee1', url: 'https://github.com/zozologin/addressbook.git']]])
        workspace=pwd()
    }
    stage('static code analysis')
    {
        echo"static code analysis"
    }
    stage('build')
    {
        echo"build the code"
    }
    stage('unit test')
    {
        echo"test the code"
    }
    stage('delivery')
    {
        echo"deliver my code"
    }
}
