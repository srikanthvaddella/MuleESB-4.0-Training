pipeline{
 agent any
 environment {
    ANYPOINT = credentials('ANYPOINT')
 }
 stages {
 	stage ('Build'){
 		steps {
 			withMaven(maven:'maven'){
 				sh 'mvn -f mule- pom.xml clean install'
 			}
 		}
 	}
 	stage ('Deploy'){
 		steps {
 			withMaven(maven:'maven'){
 				sh 'mvn -f pom.xml package deploy  -Dusername=srikanth_vaddella_01 -Dpassword=IN$BANG$W8$a -Denvironment=Development -DmuleDeploy'
 			}
 		}
 	}
 }

}
