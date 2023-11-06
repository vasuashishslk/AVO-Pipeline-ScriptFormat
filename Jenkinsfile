pipeline {
    agent any
 
 
    stages {
        stage('Build and Run') {
            steps {
                script{
                def body = '{"key":4323fdee-d08a-4333-9875-d1da84b5c591 , "executionType":asynchronous}'
                def http = new URL("https://training.avoassure.ai/execAutomation").openConnection() as HttpURLConnection
        http.setRequestMethod('POST')
        http.setDoOutput(true)
        http.setRequestProperty("Accept", 'application/json')
        http.setRequestProperty("Content-Type", 'application/json')
 
        http.outputStream.write(body.getBytes("UTF-8"))
        http.connect()
            }
        }
    }
}
}
