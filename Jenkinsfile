node{
stage ("scm checkcode")
{
git "https://github.com/sudidelahanu/Devopspipe.git"
}
stage ("mvn -package"){
def workspace=tool name: 'maven', type: 'maven'
sh "${mvnHome}/bin/mvn package "
}
stage ("email notations"){
mail bcc: '', body: '''hi 
iam s.hanuamnathareddy''', cc: '', from: '', replyTo: '', subject: 'piple line jobs', to: 'sudidelahanu6@gmail.com'
}
}
