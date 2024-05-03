pipeline{
  agent any
  stages{
    stage('Repo Checkout'){
      steps{
      checkout scmgit(branches :[ $class: 'GitSCM', [name :'*/main']], extensions : [], userRemoteConfigs : [[url:'https://github.com/Aravind0211/scmrepo.git']])
      }
    }
  }
}
