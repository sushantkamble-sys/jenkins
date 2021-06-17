`apt-get update -y`

`apt-cache search openjdk`

`apt-get install openjdk-11-jdk -y`

`java --version`

/*-------Adding Repository -----*/

`wget -q -O - https://pkg.jenkins.io/debian-stable/jenkins.io.key | sudo apt-key add -`

`sh -c 'echo deb https://pkg.jenkins.io/debian-stable binary/ > /etc/apt/sources.list.d/jenkins.list'`

`apt-get update`

`apt-get install jenkins -y`

`systemctl start jenkins`

`systemctl enable jenkins`

cat /var/lib/jenkins/secrets/initialAdminPassword
