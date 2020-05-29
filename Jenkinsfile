node{
     wrap([$class: 'BuildUser']) {
        script {
          def environment = "officedepot"
          def service = common.getDeployName()
          def workNotes = "Standard change for deploying ${service} to prod"

          println "Template: ${config.changeRequest.templateId}, CI: ${config.changeRequest.ci}, Category: ${config.changeRequest.category}, WorkNotes: ${workNotes}"

          standardChange(config.changeRequest.templateId, getStartDate(), getEndDate(), config.changeRequest.ci, BUILD_USER, environment, workNotes, config.changeRequest.category)

          println "Change control created and can be viewed here: ${env.SN_CHANGE_LINK}"
        }
      }
}
