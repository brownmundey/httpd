pipeline {
	agent {
		label {
			label "built-in"
			customWorkspace "/home/hima/23q1/"
		}
	}
	stages {
		stage ("deploy-23q1") {
			steps {
				sh "sudo chmod -R 777 /home/hima/23q1/"
				sh "ansible-playbook test1.yaml"
				
			}
		}
	}
}
