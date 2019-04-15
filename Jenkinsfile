node('master') {

	checkout scm

	stage('build') {   
		withMaven(tempBinDir: '') {
		bat label: 'mavenClean', script: 'mvn clean install -f ./DEVOPS/pom.xml'
		}	
	}

}