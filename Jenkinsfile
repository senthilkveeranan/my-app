node{
    stage('SCM Checkout'){
      git 'https://github.com/senthilkveeranan/my-app'
    }
    stage('Compile-Package'){
        // mvn Homepath
        def mvnHome = tool name: 'maven-3', type: 'maven'
        sh "${mvnHome}/bin/mvn package"
    }
    stage('Email Notifications'){
        mail bcc: '', body: '''Hi Welcome to Jenkins email alerts
        Thanks
        Senthil Veera''', cc: '', from: '', replyTo: '', subject: 'Jenkins-job', to: 'vsknalli@gmail.com,sabaa.23@gmail.com'
    
    }
}
