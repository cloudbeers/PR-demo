@Library('github.com/jglick/sample-pipeline-library@ca40387') _
node {
  checkout scm
  echo "current file: ${readFile 'file'}"
  echo "changed since the last build? ${currentBuildExt().hasChangeIn('file')}"
}
