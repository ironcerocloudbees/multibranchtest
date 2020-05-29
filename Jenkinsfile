pipeline{
     agent any
     stages{
          stage("1"){
               node{
                    wrap([$class: 'BuildUser']) {
                       script {
                            script{
                              def environment = "officedepot"
                            }
                       }
                     }
               }
          }
     }
}
