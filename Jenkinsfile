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
