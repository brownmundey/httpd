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
				sh "sudo chmod -R 777 /mnt/free/*"
				sh "ansible-playbook test1.yaml"
				
				
			}
		}
	}
}
