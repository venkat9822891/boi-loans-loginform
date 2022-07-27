node {
    stage('cont.download') {
    git 'https://github.com/venkat9822891/boi-loans-loginform.git'
}
    stage('cont.build') {
    sh 'mvn package'
}
    stage('cont.deployment') {
    deploy adapters: [tomcat8(credentialsId: 'f552cd72-0ce9-41b3-8f38-f814d5846b42', path: '', url: 'http://52.66.161.93:8080')], contextPath: '/test', war: '**/*.war'
}
    
    
}
