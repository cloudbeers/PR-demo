stage('before') {
  sleep 1
}
stage('main') {
  node {
    checkout scm
    isUnix() ? sh('ls -l') : bat('dir')
  }
}
stage('after') {
  sleep 1
}
