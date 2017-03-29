stage('Prompt') {
  input 'Ready?'
}
stage('Run') {
  node {
    checkout scm
    sh 'cat content.txt'
  }
}
