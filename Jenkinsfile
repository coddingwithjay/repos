pipeline{
  agent any
  stages{
  stage("build")
  {
    steps
    {
      echo 'building project'
      sh "\"${tool 'MSBuild-2022'}\" WebApplication1.sln /p:Configuration=Release /p:Platform=\"Any CPU\""
      
    }
  }
    stage("test")
  {
    steps
    {
      echo 'testing project'
    }
  }
    stage("deploy")
  {
    steps
    {
      echo 'deploying project'
    }
  }
  }
}
