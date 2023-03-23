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
		stage ("deploy-23q2") {
			agent {
				label {
					label "built-in"
					customWorkspace "/home/hima/23q2/"				}
			}
			steps {
				sh "sudo chmod -R 777 /home/hima/23q2/"
				sh "ansible-playbook test2.yaml"
			}
		}
	}
}
