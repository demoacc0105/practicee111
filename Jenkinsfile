pipeline {
 agent any
 tools {
 maven 'Maven3'
 jdk 'JDK17'
 }
 stages {
 stage('Checkout') {
 steps {
 git branch: 'main',url:'https://github.com/demoacc0105/practicee111.git'
 }
 }
 stage('Build') {
 steps {
 sh 'mvn clean compile'
 }
 }
 stage('Test') {
 steps {
 sh 'mvn test'
 }
 }
 stage('Package') {
 steps {
 sh 'mvn package'
 }
 }
 }
}
