pipeline {
	agent any
	triggers {
	         cron('0 0 * * *') // Mid-night build
	}
	// can also use ('H 0 * * *')         
 	stages {
 		stage("Compile") {
 			steps {
 				echo "python compile done"
 			}
 		}
 		stage("Unit test") {
 			steps {
 				sh "python3 test.py"
 			}
 		}
 	}
}

