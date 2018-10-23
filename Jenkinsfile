#!groovy

pipeline {
    agent any
    parameters {
        string(name: 'Source_Branch', defaultValue: 'Source Branch')
	booleanParam(name: 'Dryrun', defaultValue: true, description: 'Do you need Dry run?')
	string(name: 'Target_Branch', defaultValue: 'Target Branch')
    }
stages {
        stage('Merge') {
            steps {
                ##echo "Source ${params.Source_Branch}"
                ##echo "Biography: ${params.Dryrun}"
		##echo "Target ${params.Target_Branch}"
		    if (Source_Branch=July2018_Release)
		    {
	       git push https://github.com/Sachus/Std_Policy_Guidewire.git HEAD:Aug2018_Release
		       }
	    }
	}
   }
}
