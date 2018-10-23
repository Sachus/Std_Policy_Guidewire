#!groovy

pipeline {
    agent any
    parameters {
        string(name: 'Source Branch', defaultValue: 'Source Branch')
	booleanParam(name: 'Do you need a dry run', defaultValue: true)
	string(name: 'Target Branch', defaultValue: 'Target Branch')
    }
stages {
        stage('Example') {
            steps {
                echo "Source ${params.Source Branch}"
                echo "Biography: ${params.Do you need a dry run}"
		echo "Target ${params.Target Branch}"
	 }
	}
   }
}
                
