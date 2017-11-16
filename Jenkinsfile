pipeline
{
 node('slave')
stages{
stage 'build'{
   git url: 'https://github.com/jayanthich/jenkinspl.git'
     withEnv(["PATH+MAVEN=${tool 'Maven'}/bin"]) {
          sh "mvn -B clean package"
     }
     stash excludes: 'target/', includes: '**', name: 'source'
	 }
}
}
