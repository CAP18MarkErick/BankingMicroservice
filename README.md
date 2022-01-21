# BankingMicroservice
:hammer_and_wrench: SETTING UP JENKINS
1172  systemctl status jenkins
1173  apt-get  update
1174  apt-get  install  openjdk-8-jdk
1175  java -version
1176  wget -qO - https://pkg.jenkins.io/debian-stable/jenkins.io.key | apt-key add -
1177  sudo sh -c 'echo deb http://pkg.jenkins.io/debian-stable binary/ > /etc/apt/sources.list.d/jenkins.list'
1178  sudo apt-get update
1179  sudo apt-get install jenkins
1180  systemctl status jenkins
1181  sudo ufw allow 8080
1182  vi /etc/sudoers
1190  cat /var/lib/jenkins/secrets/initialAdminPassword
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


