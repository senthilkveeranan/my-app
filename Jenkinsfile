node{
    stage('SCM Checkout'){
      git 'https://github.com/senthilkveeranan/my-app'
    }
    stage('Compile-Package'){
        // mvn Homepath
        def mvnHome = tool name: 'maven-3', type: 'maven'
        sh "${mvnHome}/bin/mvn package"
    }
}
