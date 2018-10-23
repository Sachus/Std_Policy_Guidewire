#!groovy

pipeline {
    agent any
        parameters {
        string(name: 'Source_Branch', defaultValue: 'Source Branch')
	booleanParam(name: 'Dryrun', defaultValue: true, description: 'Do you need Dry run?')
	string(name: 'Target_Branch', defaultValue: 'Target Branch')
	}
stages {
        stage('Checkout') {
            steps {
    checkout([$class: 'GitSCM',
    branches: [[name: 'origin/July2018_Release']],
    extensions: [[$class: 'WipeWorkspace']],
    userRemoteConfigs: [[url: 'https://github.com/Sachus/Std_Policy_Guidewire']]
])
  stage('Merge') {
            steps {
	       git push origin/Aug2018_Release
		       }
  }
	    }
	}
   }
}
