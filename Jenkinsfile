#!groovy
sleep 15
node {
  checkout scm
  sh '''
ls -l && env | sort
'''
}
sleep 15
echo 'Here, have some fixes!'
