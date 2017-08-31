pipeline {
    agent any
    environment {
        env.PATH = "newPath/bin:${env.PATH}"
        version = '1.0' + env.BUILD_NUMBER
        currentBuild.displayName = version
    }

    stages {
        stage('Configure') {
            steps {
                echo "PATH = ${env.PATH}"
                echo "Configure End"
            }
        }
        stage('Build') {
            steps {
                // sh 'make'
                echo "End Build"
            }
        }
        stage('Test'){
            steps {
                // sh 'make check'
                // junit 'reports/**/*.xml'
                echo " End Test"
            }
        }
        stage('Deploy') {
            steps {
               // sh 'make publish'
               echo "End Deploy"
            }
        }
    }
}

/*
node('master') {

    stage('Configure') {
        env.PATH = "newPath/bin:${env.PATH}"
        version = '1.0' + env.BUILD_NUMBER
        currentBuild.displayName = version
        echo "PATH = ${env.PATH}"
        echo "Configure End"
    }

    stage('Checkout') {
        git 'https://github.com/LewChang/tooltests'
        echo "Did a Checkout"
    }

    stage('Build') {
        echo "Building, Building, Building"
    }

    stage('Archive') {
        echo  "Archive Archive Archive"
    }
}
*/