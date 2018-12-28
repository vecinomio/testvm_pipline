pipeline {
    agent any

    stages {
        stage ('creating vm') {
            steps {
                echo 'Trying to setup VM.....'
                dir('/Users/imaki/vagrant-projects/testvm') {
                    sh 'BUILD_ID=dontKillMe vagrant up'
                }    
            }
        }

    }


}
