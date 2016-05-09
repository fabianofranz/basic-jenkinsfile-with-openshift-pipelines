node('agent'){
  stage 'frontend'
  def builder = new com.openshift.jenkins.plugins.pipeline.OpenShiftBuilder("https://192.168.2.200:8443", "ruby-sample-build", "default", "", "false", "", "", "false", "")
  step builder
  echo 'frontend built'

  stage 'database'
  echo 'database already built, nothing to do'
}
