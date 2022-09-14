## check hadoop yarn web proxy path
ll /usr/hdp/3.1.4.0-315/hadoop-yarn/.//hadoop-yarn-server-web-proxy-3.1.1.3.1.4.0-315.jar -> 
ll /usr/hdp/3.1.4.0-315/hadoop-yarn/.//hadoop-yarn-server-web-proxy.jar

# tut
```
# backup old lib
mv /usr/hdp/3.1.4.0-315/hadoop-yarn/.//hadoop-yarn-server-web-proxy-3.1.1.3.1.4.0-315.jar /usr/hdp/3.1.4.0-315/hadoop-yarn/.//
hadoop-yarn-server-web-proxy-3.1.1.3.1.4.0-315.jar_bk

# update new lib & rename
scp lib/hadoop-yarn-server-web-proxy-3.4.0-SNAPSHOT.jar $hadoop_lib;
mv /usr/hdp/3.1.4.0-315/hadoop-yarn/.//hadoop-yarn-server-web-proxy-3.4.0-SNAPSHOT.jar /usr/hdp/3.1.4.0-315/hadoop-yarn/.//hadoop-yarn-server-web-proxy-3.1.1.3.1.4.0-315.jar

# update lib driver
scp lib/commons-lang-2.6.jar $dirver_lib
scp lib/tungtvauth-1.1.0.jar $diver_lib
```

## user:pass for test
admin:1