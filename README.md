# BankingMicroservice

:hammer_and_wrench: <b>SETTING UP JENKINS</b> <br /> <br />
systemctl status jenkins <br />
apt-get  update <br />
apt-get  install  openjdk-8-jdk <br /> 
java -version <br /> 
wget -qO - https://pkg.jenkins.io/debian-stable/jenkins.io.key | apt-key add - <br /> 
sudo sh -c 'echo deb http://pkg.jenkins.io/debian-stable binary/ > /etc/apt/sources.list.d/jenkins.list' <br /> 
sudo apt-get update <br /> 
sudo apt-get install jenkins <br /> 
systemctl status jenkins <br /> 
sudo ufw allow 8080 <br /> 
vi /etc/sudoers <br /> 
cat /var/lib/jenkins/secrets/initialAdminPassword <br />

:hammer_and_wrench: <b>SETTING UP GIT</b> <br /> <br />
git --version <br />
apt purge git -y <br />
add-apt-repository ppa:git-core/ppa <br />
apt update <br />
apt install git <br /> 
git clone https://github.com/CAP18MarkErick/BankingMicroservice.git <br />
cd BankingMicroservice <br />

:hammer_and_wrench: <b>INSTALLING MAVEN PROJECT</b> <br /> <br />
apt update <br /> 
apt install maven -y <br /> 
mvn --version <br />
mvn archetype:generate <br /> 
cd capstone <br /> 
mvn compile <br /> 
mvn clean <br />
mvn package <br />

:hammer_and_wrench: <b>GIT COMMANDS</b> <br /> <br />
git pull origin master <br />
git add . <br />
git status <br />
git commit -m "Banking Microservice project" <br />
git config --global user.name CAP18MarkErick <br />
git commit -m "Banking Microservice project" <br />
git push origin master <br />
git config --global credential.helper store <br />
git config --global credential.helper cache <br />
ssh-keygen <br /> 
cat /root/.ssh/id_rsa.pub <br />
git push <br />
git --no-pager log > log.txt <br />
ls <br />
cat log.txt <br />
git rm 1.txt 2.txt <br />
git commit -m "1.txt and 2.txt deleted" <br />
git push <br />


