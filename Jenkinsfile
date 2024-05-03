pipeline{
  agent any{
    stage('Repo Checkout'){
      checkout scmgit(branches :[[name :'*/main']], extensions : [], userRemoteConfigs : [[https://github.com/Aravind0211/scmrepo.git]])
    }
  }
}
