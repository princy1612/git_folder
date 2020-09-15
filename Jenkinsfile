node
{
    stage("checkout scm")
    {
        echo("check the scm")
        checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[credentialsId: '911c2672-2096-4046-9317-a31226659fbc', url: 'https://github.com/princy1612/git_folder.git']]])
          }
    stage ("build")
    {
        echo("build the  code")
        bat 'git_folder\\main'
    }
    stage ("test")
    {
       
        echo("test the code")
        bat 'git_floder\\main>$ javac BankAppln.java'
    }
}  
      
