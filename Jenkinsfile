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
				
			}
		}
	}
}
