#!groovy
pipeline {
   agent any
  def handleCheckout = {
	sh "echo 'Checking out a merge request...'"
	def credentialsId = scm.userRemoteConfigs[0].credentialsId
	checkout ([
		$class: 'GitSCM'}
    }
