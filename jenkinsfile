node {
    def mvnHome = tool 'MVN' 

    stage('Checkout') {
        
       git branch: 'main', credentialsId: '42a8cd56-507b-461f-810e-d0fe01264c56', url: 'https://github.com/Ainnikumar/maven.git/'
    }

    stage('Validate') {
       
        bat "${mvnHome}\\bin\\mvn validate"
    }

    stage('Clean') {
        
        bat "${mvnHome}\\bin\\mvn clean"
    }

    stage('Compile') {
       
        bat "${mvnHome}\\bin\\mvn compile"
    }

    stage('Test') {
        
        bat "${mvnHome}\\bin\\mvn test"
    }

    stage('Package') {
       
        bat "${mvnHome}\\bin\\mvn package"
    }

    stage('Verify') {
        
        bat "${mvnHome}\\bin\\mvn verify"
    }

    stage('Install') {
        
        bat "${mvnHome}\\bin\\mvn install"
    }

    stage('Site') {
        
        bat "${mvnHome}\\bin\\mvn site"
    }
}
