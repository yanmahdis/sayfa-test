node {
  stage('Check Environment') {
            sh '''
               env
               node --version
               npm --version
               git --version
            '''

            println "[DEBUG-DeployStage] - aws_creds = ${env.BRANCH_NAME}"
  }
}