pipeline {
   environment {

      // rockhopper vagrantfiles scripts repository
      GITHUB_REPO_VAGRANT = 'ssh://git@git.intra.lutron.com:7999/vc/rockhopper-vagrantfiles.git'

   }
    agents any
    stages {
        stage('stage-1 test-vagrant') {
            steps {
                script {
                    utility.checkoutRepository('vagrantfiles',
                                               GITHUB_REPO_VAGRANT,
                                               'master')
                    public VagrantUpCommand(String vagrantFile,
                                            String vagrantVm,
                                            boolean destroyOnError,
                                            String provider,
                                            boolean dontKillMe)
                }
            }
        }
    }
}