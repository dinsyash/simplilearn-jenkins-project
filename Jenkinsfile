pipeline {
	agent any
	stages {
		stage('Compile') {
			steps {
				echo "compiled successfully"
			}
		}
		stage('JUnit') {
			steps {
				echo "JUnit passed successfully"
			}
		}
		stage('Quality-Gate') {
			steps {
				echo "Quality gate passed successfully"
				/**/
			}
		}
		stage('Deploy') {
			steps {
				echo "Pass!!"
			}
		}
	}
	post {
		always {
			echo "This will always run"
		}
		success{
			echo "This will run only if successful"  
		}
		failure{
			echo "This will run only if failed"
		}
		unstable{
			echo "This will only run if the run was marked as unstable"
		}
		changed{
			echo "This will run only if the state of the pipeline has changed"
		}
	}
}