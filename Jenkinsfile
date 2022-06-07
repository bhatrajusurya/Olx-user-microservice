  pipeline {

agent any



stages {



stage('compile') {

steps {

bat 'mvn clean compile'

}

}

stage('Run') {

steps {

bat 'mvn package'

}

}

stage('test report using jacoco') {

steps {

jacoco()

}

}

stage('Building Docker Image') {

steps {

echo 'Building Docker Image'

}

}

}

}
