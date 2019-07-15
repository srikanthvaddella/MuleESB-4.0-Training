pipeline{
 agent any
 environment {
    ANYPOINT = credentials('anypoint')
 }
 stages {
 	
        stage('Build') { 
            steps {
                sh 'mvn -B -DskipTests clean install' 
            }
        }

 }

}
