node('agent'){
  stage 'frontend'
  def builder = new com.openshift.jenkins.plugins.pipeline.OpenShiftBuilder("", "frontend", "default", "", "false", "", "", "false", "") 
  step builder
  echo 'frontend built'

  stage 'database'
  echo 'database built'
}
