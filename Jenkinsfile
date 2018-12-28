pipeline {
    agent any

    stages {
        stage ('creating vm') {
            steps {
                echo 'Trying to setup VM.....'
                dir('/Users/imaki/vagrant-projects/testvm') {
                    build 'test1_up'
                }    
            }
        }

    }


}
