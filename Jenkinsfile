pipeline { 
    agent any 
    stages { 
        stage('Checkout') { 
            steps { 
                git url:'<你的GitHub项目地址>', branch: 'main' 
            } 
        } 
        stage('Install') { 
            steps { 
                bat 'pip install -r requirements.txt' 
            } 
        } 
        stage('Test') { 
            steps { 
                bat 'pytest' 
            } 
        } 
    } 
}
