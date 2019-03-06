pipeline { 
    agent any 

    stages {
        stage('Version Control') { 
            steps {
		withMaven(maven : 'Maven_3_6_0') {
                    sh 'mvn clean compile' 
		}
            }
        }
        stage('Build Stage') { 
            steps {
		withMaven(maven : 'Maven_3_6_0') {
                    sh 'mvn clean compile' 
		}
            }
        }
        stage('Unit test'){
            steps {
		withMaven(maven : 'Maven_3_6_0') {
                    sh 'mvn clean compile' 
		} 
            }
        }
        stage('Deploy stage') {
            steps {
		withMaven(maven : 'Maven_3_6_0') {
                    sh 'mvn clean compile' 
		}
            }
        }
        stage('Deploy') {
            steps {
		withMaven(maven : 'Maven_3_6_0') {
                    sh 'mvn clean compile' 
		}
            }
        }
        stage('Auto Test stage') {
            steps {
		withMaven(maven : 'Maven_3_6_0') {
                    sh 'mvn clean compile' 
		}
            }
        }
        stage('Deploy to Production stage') {
            steps {
		withMaven(maven : 'Maven_3_6_0') {
                    sh 'mvn clean compile' 
		}
            }
        }
        stage('Measure + Validate stage') {
            steps {
		withMaven(maven : 'Maven_3_6_0') {
                    sh 'mvn clean compile' 
		}
            }
        }
    }
}
