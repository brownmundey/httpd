pipeline {
	agent {
		label {
			label "built-in"
			customWorkspace "/mnt/httpd"
		}
	}
	stages {
		stage ("23q1") {
			steps {
				sh "docker run -itdp 80:80 --name 23Q1 httpd"
				sh "docker cp /mnt/httpd/index.html 23Q1:/usr/local/apache2/htdocs"
			}
		}
	}
}
