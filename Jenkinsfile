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
	 //agent any
	 agent {docker { image 'maven:3.6.3' } }
	 stages{
		 stage('Build'){
			 steps {
				 sh "maven --version"  // for shell executuon 
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
 post{
	 always{
		 echo "It will run always"
	 }
	 success{
		 echo "i run when success"
	 }
	 failure{
		 echo "i execute when it fails"
	 }
	 changed{
		 echo "This will change when change in some build like build jenckis 4 and next build 5 have some diff"
	 }
 }