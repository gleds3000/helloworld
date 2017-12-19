stage 'Checkout'
 node('slave') {
  sh 'echo teste'
  //deleteDir()
 // checkout scm
 }
// This shows a simple build wrapper example, using the AnsiColor plugin.
stage 'Cores'
node {
    // This displays colors using the 'xterm' ansi color map.
    ansiColor('xterm') {
        // Just some echoes to show the ANSI color.
        stage "\u001B[31mI'm Red\u001B[0m Now not"
    }
}
  post {
        failure {
            mail to: 'gleds3000@gmail.com', subject: 'Pipeline falhou em local', body: "${env.BUILD_URL}"
        }
    }
