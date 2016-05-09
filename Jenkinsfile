node('agent'){
  stage 'frontend'
  def apiURL = 'https://192.168.2.200:8443'
  def buildConfig = 'ruby-sample-build'
  def namespace = 'default'
  step new com.openshift.jenkins.plugins.pipeline.OpenShiftBuilder(apiURL, buildConfig, namespace, '', 'false', '', '', 'false', '')
  echo 'frontend built'

  stage 'database'
  echo 'database already built, nothing to do'
}
