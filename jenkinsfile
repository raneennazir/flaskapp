pipeline{
agent any

stages{
stage("Checkout Code") {
steps{
git branch:'main', url:'https://github.com/raneennazir/flaskapp.git'
}
}
stage('Install Dependencies'){
steps{
sh 'pip install -r requirements.txt'
}
}
stage('Run Flask App') {
steps {
sh 'nohu python app.py &'
}
}
}
}
