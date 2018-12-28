pipeline {
    agent any

    stages {
        stage ('Checkout SCM') {
            steps {
                checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [[$class: 'RelativeTargetDirectory', relativeTargetDir: '/Users/imaki/vagrant-projects/testvm']], submoduleCfg: [], userRemoteConfigs: [[url: 'https://github.com/vecinomio/testvm_pipline.git']]])
            }    
        }
        stage ('creating vm') {
            steps {
                echo 'Trying to setup VM.....'
                
                // Change to the project dir
                dir('/Users/imaki/vagrant-projects/testvm') {
                    
                    // Start freestyle job that create VM using vagrant plugin
                    build 'test1_up'
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
