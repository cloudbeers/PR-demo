stage('before') {
  sleep 2
}
stage('main') {
  node {
    checkout scm
    isUnix() ? sh('ls -l') : bat('dir')
  }
}
stage('after') {
  sleep 2
}
