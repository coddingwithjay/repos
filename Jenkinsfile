pipeline{
  agent any
  stages{
  stage("build")
  {
    steps
    {
      echo 'building project'
      bat "\"${tool 'MSBuild-v4.0.30319'}\" WebApplication1.sln /p:Configuration=Release /p:Platform=\"Any CPU\""
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
