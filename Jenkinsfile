node{
          stage("1"){
               node{
                    checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], gitTool: 'Default', submoduleCfg: [], userRemoteConfigs: [[url: 'https://github.com/ironcerocloudbees/multibranchtest.git']]])
               }
          }
}
