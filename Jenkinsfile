pipeline {
    agent {
        docker {
            image 'maven:3.3.3' 
            args '-v /Users/zhuxiuwei/.m2:/root/.m2' 
        }
    }
    stages {
        stage('Build') { 
            steps {
                sh 'mvn -B -DskipTests clean package' 
            }
        }
    }
}
