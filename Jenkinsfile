pipeline {
  agent any
  stages {
    stage('Server') {
      parallel {
        stage('Server') {
          agent {
            docker {
              image 'maven:3.5-jdk-8-slim'
            }

          }
          steps {
            sh '''echo "Building the code of our server, be patient"






mvn 
-version

mkdir-p target
touch "target/server.war"'''
            stash(name: 'server', includes: '**/*.war')
          }
        }
        stage('client') {
          agent {
            docker {
              image 'node:6'
              args '-u 0:0'
            }

          }
          steps {
            sh '''echo "Building the code for a client..."
npm install --save react 
mkdir -p dist 
cat > dist/index.html <<EOF 
Hello, welcome to my pipeline testing!!! 
EOF 
touch "dist/client.js"'''
          }
        }
      }
    }
  }
}