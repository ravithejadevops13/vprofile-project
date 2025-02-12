pipeline{

    agent any

    tools{
        jdk "JDK17"
        maven "MAVEN3.9"
    }

    environment{
        SNAP_REPO = 'vprofile-snapshot'
		NEXUS_USER = 'admin'
		NEXUS_PASS = 'admin123'
		RELEASE_REPO = 'vprofile-release'
		CENTRAL_REPO = 'maven-central'
		NEXUSIP = '52.91.246.145'
		NEXUSPORT = '8081'
		NEXUS_GRP_REPO = 'vpro-maven-group'
        NEXUS_LOGIN = 'nexuslogin'


    }

    stages{

        stage("Build"){
            steps{
                sh 'mvn -s settings.xml -DskipTests install'
            }
        }
    }





}