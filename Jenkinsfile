@Library('github.com/jglick/sample-pipeline-library@b3acaf4')
node {
  checkout scm
  echo "current file: ${readFile 'file'}"
  echo "changed since the last build? ${currentBuildExt().hasChangeIn('file')}"
}
