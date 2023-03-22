pipeline {
	agent {
		label {
			label "built-in"
			customWorkspace "/etc/ansible/"
		}
	}
	stages {
		stage ("deploy-to-hosts") {
			steps {
				sh "ansible-playbook test1.yaml
				
			}
		}
	}
}
