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


1194  git --version
1201  apt purge git -y
1202  add-apt-repository ppa:git-core/ppa
1203  apt update
1204  apt install git
1205  git clone https://github.com/CAP18MarkErick/BankingMicroservice.git
1208  cd BankingMicroservice
1209  apt update
1210  apt install maven -y
1211  mvn --version
1213  cd capstone
1215  mvn compile
1241  mvn clean
1242  mvn package
1269  git pull origin master
1272  git add .
1273  git status
1274  git commit -m "Banking Microservice project"
1275  git config --global user.name CAP18MarkErick
1276  git commit -m "Banking Microservice project"
1277  git push origin master
1284  git config --global credential.helper store
1285  git config --global credential.helper cache
1291  ssh-keygen
1292  cat /root/.ssh/id_rsa.pub
1293  git push
1297  git --no-pager log > log.txt
1298  ls
1299  cat log.txt
1300  git rm 1.txt 2.txt
1301  git commit -m "1.txt and 2.txt deleted"
1302  git push


