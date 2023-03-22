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
				sh "sudo cd /"
				sh "sudo chmod -R 777 /mnt"
				sh "ansible-playbook test1.yaml"
				
				
			}
		}
	}
}
