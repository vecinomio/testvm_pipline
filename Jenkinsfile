pipeline {
    agent any

    stages {
        stage ('creating vm') {
            steps {
                echo 'Trying to setup VM.....'
                
                // Change to the project dir
                dir('/Users/imaki/vagrant-projects/testvm') {
                    sh 'vagrant up'
                }    
            }
        }
        stage ('Tests') {
            steps {
                echo 'Trying some tests'
            }    
        }
        stage ('Deploy') {
            steps {
                echo 'Deploy something'
            }    
        }

    }


}
