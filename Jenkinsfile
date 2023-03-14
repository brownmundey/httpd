pipeline {
	agent {
		label {
			label "built-in"
			customWorkspace "/mnt/httpd-3"
		}
	}
	stages {
		stage ("23q3") {
			steps {
				sh "docker run -itdp 802:80 --name 23Q3 httpd"
				sh "docker cp /mnt/httpd-3/index.html 23Q3:/usr/local/apache2/htdocs"
				sh "docker exec -it 23Q3 bash"
				sh "chmod -R 777 htdocs"
			}
		}
	}
}
