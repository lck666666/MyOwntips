# MyOwntips
## MAC换源
``~ pip install ipython -i http://mirrors.aliyun.com/pypi/simple/ --trusted-host mirrors.aliyun.com``

https://blog.csdn.net/qq_43340659/article/details/82948529?depth_1-utm_source=distribute.pc_relevant.none-task&utm_source=distribute.pc_relevant.none-task

https://blog.csdn.net/jiachen0212/article/details/81022079
## Cifar10 jpg数据集
https://blog.csdn.net/guohuifengby/article/details/62424299

## iptables
```shell
sudo iptables -t nat 
sudo iptables -t nat -A POSTROUTING ! -d 192.168.204.0/25 -j MASQUERADE
sudo iptables -t nat -A POSTROUTING -s 192.168.204.128/25 -j MASQUERADE
```
Chain PREROUTING (policy ACCEPT)

target     prot opt source               destination

Chain INPUT (policy ACCEPT)

target     prot opt source               destination

Chain POSTROUTING (policy ACCEPT)

target     prot opt source               destination

MASQUERADE  all  --  anywhere            !192.168.204.0/25

Chain OUTPUT (policy ACCEPT)

target     prot opt source               destination
