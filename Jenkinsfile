#!groovy

pipeline {
    agent any
	def a= "July2018_Release"
	def b="Target_Branch"
        parameters {
        string(name: 'Source_Branch', defaultValue: 'Source Branch')
	booleanParam(name: 'Dryrun', defaultValue: true, description: 'Do you need Dry run?')
	string(name: 'Target_Branch', defaultValue: 'Target Branch')
    }
stages {
        stage('Merge') {
            steps {
               /* ##echo "Source ${params.Source_Branch}"
                ##echo "Biography: ${params.Dryrun}"
		##echo "Target ${params.Target_Branch}"*/
		    if ($a)
	       git push https://github.com/Sachus/Std_Policy_Guidewire.git HEAD:Aug2018_Release
		       }
		    else {
		    println("The value is not acceptable");
		    }
	    }
	}
   }
}
