node('master')
{
stage('continuousdownload_master')
{
git 'https://github.com/Shaj-2020/Maven1.git'
}
stage('continuousBuild_master')
{
sh label: '', script: 'mvn package'
}
}

