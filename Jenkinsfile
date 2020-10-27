node{
          stage("1"){
               node{
                    echo "Checkout phase"
                    checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[url: 'https://github.com/ironcerocloudbees/multibranchtest.git']]])
               }
          }
}
