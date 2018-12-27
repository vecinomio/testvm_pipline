pipeline {
    agent any

    stages {
        stage ('creating vm') {
            steps {
                echo 'Trying to setup VM.....'
                sh 'cd /Users/imaki/vagrant-projects/testvm/ && BUILD_ID=dontKillMe vagrant up'
                
            }
        }

    }


}
