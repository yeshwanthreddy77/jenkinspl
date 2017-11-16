pipeline
{
 node('slave')
stages{
stage 'build'
	{
   git 'git@github.com:jayanthich/jenkinspl.git'
     
     stash excludes: 'target/', includes: '**', name: 'source'
	 }
}
}
