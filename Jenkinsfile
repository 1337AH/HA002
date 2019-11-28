pipeline {
agent {docker 'maven:3-alpine'}
stages {
stage('Build') {
steps {
sh 'mvn clean package'
echo "this is Build stage"
}
}

stage ('Test: integration-&-quality') {
steps {

echo "this is I/Q stage"
}
}
stage ('Test: functional') {
steps {

echo "this is functional stage"
}
}
stage ('Test: load-&-security') {
steps {

echo "this is security stage"
}
}
stage ('Approval') {
steps {

echo "this is approval stage"
}
}
stage ('Deploy:prod') {
steps {

echo "this is deploy stage"
}
}
}
}
