# Employee-Management-System-React-JS-Spring-Boot-MySQL
Employee Management System (React JS + Spring Boot + MySQL)

#Java and maven setup

sudo apt update && sudo apt upgrade
sudo apt install openjdk-17-jre
sudo apt install openjdk-17-jdk

wget https://dlcdn.apache.org/maven/maven-3/3.9.1/binaries/apache-maven-3.9.1-bin.tar.gz
tar -xvf apache-maven-3.9.1-bin.tar.gz
sudo mv apache-maven-3.9.1 /opt/
sudo chown -R $USER:$USER /opt/apache-maven-3.9.1


sudo nano ~/.bashrc

#SET JAVA_HOME PATH

JAVA_HOME=/usr/lib/jvm/java-17-openjdk-amd64
MAVEN_HOME=/opt/apache-maven-3.9.1

export JAVA_HOME
export MAVEN_HOME

PATH=$JAVA_HOME/bin:$MAVEN_HOME/bin:$PATH

export PATH


. ~/.bashrc

echo $JAVA_HOME
echo $MAVEN_HOME

jave --version
mvn --version

How to install mysql server and set the password for root user
sudo apt update
sudo apt install mysql-server -y
sudo systemctl start mysql.service
sudo systemctl status mysql.service
sudo mysql
ALTER USER 'root'@'localhost' IDENTIFIED WITH mysql_native_password BY 'root';
exit
mysql -u root -p


npm i
npm start

java -jar jarfilename

