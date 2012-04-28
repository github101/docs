### Hadoop 伪分布式开发环境

##### 创建账号 Hadoop账号
<pre>
groupadd hadoop
mkdir /home/hadoop
useradd -g hadoop -d /home/hadoop -s /bin/bash hadoop

passwd hadoop

cp /home/xxx/.bashrc /home/hadoop

chown -R hadoop:hadoop /home/hadoop

su - hadoop
 
ssh-keygen -t rsa
 
cat ~/.ssh/id_rsa.pub >> ~/.ssh/authorized_keys
chmod 600 ~/.ssh/authorized_keys 
</pre>

#### 设置个人Java运行环境变量，该安装包自带了JDK-1.6.u26版本


##### 在.bashrc尾部添加jdk环境变量
<pre>
export JAVA_HOME=/home/hadoop/jdk1.6.0_26
export CLASSPATH=.:$CLASSPATH:$JAVA_HOME/lib/dt.jar:$JAVA_HOME/lib/tools.jar
export PATH=$JAVA_HOME/bin:$PATH

source .bashrc
</pre>

##### 软件包现在地址

<http://dl.dropbox.com/u/62934464/hadoop_env.tar.gz/>

##### 解压hadoop_env.tar.gz文件
<pre>
cd hadoopbin/hadoop namenode -format
bin/start-all
</pre>
