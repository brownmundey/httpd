pipeline {
	agent {
		label {
			label "built-in"
			customWorkspace "/mnt/free"
		}
	}
	stages {
		stage ("deploy-to-hosts") {
			steps {
				sh "ansible-playbook test1.yaml"
				sh "sudo cd /"
				sh "sudo chmod -R 777 mnt/"
				
			}
		}
	}
}
