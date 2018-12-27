pipeline {
    agent any

    stages {
        stage ('creating vm') {
            steps {
                echo 'Trying to setup VM.....'
                sh 'BUILD_ID=dontKillMe cd /Users/imaki/vagrant-projects/testvm/ && vagrant up'
                
            }
        }

    }


}
