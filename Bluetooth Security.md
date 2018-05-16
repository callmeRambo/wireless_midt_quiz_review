# Bluetooth Security
开放的无线数据交换协议，适合短距离移动设备
* Open wireless protocol for exchanging data over short distances from fixed and mobile devices, creating personal area network.
* A reliable wireless protocol for voice and data transmission
## 蓝牙
* Bluetooth Special Interest Group (SIG)
* Founded in Spring 1998
* By Ericsson, Intel, IBM, Nokia, Toshiba
* Now more than 2,000 organizations have joined the SIG
### 1.特性
* 自动链接
* Topology is established on a temporary and random basis
拓扑结构建立
* Up to eight Bluetooth devices may be networked together in a master-slave
relationship to form a piconet
主客机最多八个
```
• One is master, which controls and sets up the network (piconet)
• Two or more piconet interconnected to form a scatter net
• Only one master for each piconet
• A device can’t be masters for two piconet
• The slave of one piconet can be the master of another piconet
```
master : piconet = 1:1
piconet : scatter net = n : 1
slave : piconet = m : n
### 2. Security Issues
```

```