#!groovy
stage 'Set-up'
sleep 15
node {
  checkout scm
  sh 'ls -l'
}
sleep 15
echo 'Have some fixes!'
stage 'Kick-off'
try {
triggerRemoteJob mode: [$class: 'TrackProgressAwaitResult', scheduledTimeout: [timeoutStr: ''], startedTimeout: [timeoutStr: ''], timeout: [timeoutStr: '1d'], whenFailure: [$class: 'StopAsFailure'], whenScheduledTimeout: [$class: 'ContinueAsIs'], whenStartedTimeout: [$class: 'ContinueAsIs'], whenTimeout: [$class: 'ContinueAsFailure'], whenUnstable: [$class: 'ContinueAsUnstable']], remotePathMissing: [$class: 'StopAsFailure'], remotePathUrl: 'cjp:///cje/org/PR-demo/master'
} catch (NoSuchMethodError _) {
    echo 'Not running on CJOC'
}
