#!groovy

pipeline {
    agent any
    parameters {
        string(name: 'Source_Branch', defaultValue: 'Source Branch')
	booleanParam(name: 'Dryrun', defaultValue: true, description: 'Do you need Dry run?')
	string(name: 'Target_Branch', defaultValue: 'Target Branch')
    }
stages {
        stage('Example') {
            steps {
                echo "Source ${params.Source_Branch}"
                echo "Biography: ${params.Dryrun}"
		echo "Target ${params.Target_Branch}"
	 }
	}
   }
}
                
