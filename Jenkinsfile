pipeline {
	agent {
		label {
			label "built-in"
			customWorkspace "/home/hima/23q2/"
		}
	}
	stages {
		stage ("deploy-to-hosts") {
			steps {
				sh "sudo chmod -R 777 /home/hima/23q2/"
				sh "ansible-playbook test2.yaml"
				
			}
		}
	}
}
