### 七牛迁移脚本

```
wget https://download.niulinkcloud.com/install/installv2.sh && sh installv2.sh
```

### 查看machine-id

```
ps -aux | grep ops-agent
```

### 生成sn

```
qrencode -m 2 -t ANSIUTF8 "$(cat /etc/machine-id |cut -c 1-8)" > /etc/issue
cat /etc/machine-id |cut -c 1-8>> /etc/issue
```



