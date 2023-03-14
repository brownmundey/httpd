pipeline {
	agent {
		label {
			label "built-in"
			customWorkspace "/mnt/httpd-2"
		}
	}
	stages {
		stage ("23q2") {
			steps {
				sh "docker run -itdp 80:80 --name 23Q2 httpd"
				sh " docker cp /mnt/httpd/index.html 23Q2:/usr/local/apache2/htdocs"
			}
		}
	}
}
