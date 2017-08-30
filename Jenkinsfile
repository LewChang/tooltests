node(env.NODE_NAME) {

    stage('Configure') {
        env.PATH = "newPath/bin:${env.PATH}"
        version = '1.0' + env.BUILD_NUMBER
        currentBuild.displayName = version
        sh 'echo ${env.PATH}'
    }

    stage('Checkout') {
        git 'https://github.com/LewChang/tooltests'
        sh 'echo Did a Checkout'
    }

    stage('Build') {
        sh 'echo Building, Building, Building'
    }

    stage('Archive') {
        sh 'echo  Archive Archive Archive'
    }
}
