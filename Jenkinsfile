pipeline {
	agent {
		label {
			label "built-in"
			customWorkspace "/mnt"
		}
	}
	stages {
		stage ("deploy-to-hosts") {
			steps {
				sh "sudo chmod -R 777 /mnt/*"
				sh "ansible-playbook test2.yaml"
				
				
			}
		}
	}
}
