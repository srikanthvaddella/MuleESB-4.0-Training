pipeline{
 agent any
 environment {
    ANYPOINT = credentials('anypoint')
 }
 stages {
 	stage ('Build'){
 		steps {
 			withMaven(maven:''){
 				sh 'mvn -f mule- pom.xml clean install'
 			}
 		}
 	}

 }

}
