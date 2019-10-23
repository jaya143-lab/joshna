node('master') {
    stage('scm') {
        checkout scm
    }
    stage('build') {
        withMaven(jdk: '1.8.0_221', maven: 'Maven3.5.3') {
            sh 'mvn clean install'
        }
    }
}
