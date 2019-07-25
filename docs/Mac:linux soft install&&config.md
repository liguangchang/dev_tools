## Mac/linux soft install&&config

### 1.jdk

```
export JAVA_HOME=/Library/Java/JavaVirtualMachines/jdk1.8.0_211.jdk/Contents/Home 
export CLASSPAHT=.:$JAVA_HOME/lib/dt.jar:$JAVA_HOME/lib/tools.jar 
export PATH=$JAVA_HOME/bin:$PATH:
```

### 2.mysql

```
PATH=$PATH:/usr/local/mysql/bin
```

### 3.git

```
git config --global user.name ""
git config --global user.email ""
cd ~/.ssh
生成密匙
ssh-keygen -t rsa -C "macbookpro"
```

### 4.jmeter

```
export JMETER_HOME=
export PATH=$JAVA_HOME/bin:$PATH:.:$JMETER_HOME/bin:$PATH
export CLASSPATH=.:$JAVA_HOME/lib/dt.jar:$JAVA_HOME/lib/tools.jar:$JMETER_HOME/lib/ext/ApacheJMeter_core.jar:$JMETER_HOME/lib/jorphan.jar:$JMETER_HOME/lib/logkit-2.0.jar
启动 jmeter
中文设置 修改 bin/jmeter.properties language=zh_CN
```

### 5.rabbitmq

```
brew install rabbitmq
开启插件
/sbin rabbitmq-plugins enable rabbitmq_management
关闭 
rabbitmqctl stop_app
重置 
rabbitmqctl reset
启动 
rabbitmqctl start_app
```

