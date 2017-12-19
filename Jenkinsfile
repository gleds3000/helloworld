//stage 'Checkout'
 //node('slave') {
  //sh 'echo teste'
  //deleteDir()
 // checkout scm
 //}
// This shows a simple build wrapper example, using the AnsiColor plugin.

}
  post {
        failure {
            mail to: 'gleds3000@gmail.com', subject: 'Pipeline falhou em local', body: "${env.BUILD_URL}"
        }
    }
