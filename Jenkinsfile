node('docker') {
  def image = docker.image('node')
  image.pull()
  image.inside {
    try {
      stage('Check Environment') {

            sh '''
               env
               node --version
               npm --version
               git --version
            '''
      }   
    }
    catch (caughtError) {
      println caughtError
    }
  }
}