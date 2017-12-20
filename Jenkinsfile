stage 'Checkout'
 node('master') {
  //sh 'echo teste'
  bat 'echo esse foi o build numero: ${BUILD_NUMBER}'
}
 post {
        failure {
            mail to: 'gleds3000@gmail.com', subject: 'Pipeline falhou em local', body: "${env.BUILD_URL}"
        }
    }
