pipeline {
	agent {
		label {
			label "built-in"
			customWorkspace "/home/hima/23q1/"
		}
	}
	stages {
		stage ("deploy-to-hosts") {
			steps {
				sh "sudo chmod -R 777 /home/hima/23q1/"
				sh "ansible-playbook test1.yaml"
				
			}
		}
	}
}
