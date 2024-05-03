pipeline{
  agent any
  stages{
    stage('Repo Checkout'){
      steps{
      checkout scmgit([ $class: 'GitSCM',branches :[[name :'*/main']], extensions : [], userRemoteConfigs : [[url:'https://github.com/Aravind0211/scmrepo.git']]])
      }
    }
  }
}
