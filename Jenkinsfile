//scripted
node {
	stage('Build') {
		echo "Build"
	}
	stage('Test') {
		echo "Test"
	}
}
 // declaritive
 pipeline{
	 agent any
	 stages{
		 stage('Build'){
			 steps {
				 echo "Build"
			 }
		 }
		 stage('Test'){
			 steps {
				 echo "Test"
			 }
		 }
	 }
 }