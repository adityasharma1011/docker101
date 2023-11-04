# Install Oracle JDK on Linux

Login as root
mkdir /opt/java-install

## Download Oracle rpm
wget https://download.oracle.com/java/19/archive/jdk-19.0.2_linux-x64_bin.rpm

chmod +x jdk-19.0.2_linux-x64_bin.rpm

yum install jdk-19.0.2_linux-x64_bin.rpm


##Create a file /etc/profile.d/java.sh with following contents 

export JAVA_HOME=/usr/lib/jvm/jdk-19-oracle-x64

export PATH=$PATH:$JAVA_HOME/bin

