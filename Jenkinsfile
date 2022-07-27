node {
    stage('cont.download') {
    git 'https://github.com/venkat9822891/boi-loans-loginform.git'
}
    stage('cont.build') {
    sh 'mvn package'
}
    stage('cont.deployment') {
    deploy adapters: [tomcat8(credentialsId: '3f09ca4c-3eb9-4dea-a467-c8a06e8436f4', path: '', url: 'http://172.31.45.215:8080')], contextPath: '/apps-dev', war: '**/*.war'
}


}
