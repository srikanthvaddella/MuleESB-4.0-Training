pipeline{
 agent any
 environment {
    ANYPOINT = credentials('anypoint')
 }
 stages {
 	stage ('Build'){
 		steps {
 			withMaven(maven:'maven'){
 				sh 'mvn -f mule- pom.xml clean install'
 			}
 		}
 	}

 }

}
