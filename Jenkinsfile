node{
    stage('SCM Checkout'){
      git 'https://github.com/senthilkveeranan/my-app'
    }
    stage('Compile-Package'){
      sh 'mvn package'
    }
}
