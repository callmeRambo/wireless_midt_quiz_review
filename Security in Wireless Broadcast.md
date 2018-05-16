# 2
## ECDH 
ECDH是EC是“ elliptic curves”的意思，DH是“ Diffie-Hellman”的意思。它实际上是密钥协商算法，而不是加解密算法。 
该算法可以用来解决如下问题：两端（Alice 和 Bob）想要安全的交换信息并且第三方不能获取到该信息。当然这是TLS协议中的目的之一，我们给出一个例子。 
（其实下面的描述其实是ECDHE,而不是ECDH）

（1）Alice 和 Bob 生成他们自己的私钥和公钥，即Alice 有 da、Ha = da*G；Bob有db、Hb = db *G 

（2）Alice把Ha发给Bob，Bob把Hb发给Alice。这样Alice 有da,Ha,Hb，Bob有db,Ha,Hb

（3）Alice计算S = da*Hb（即自己的私钥乘上Bob的公钥），同样的，Bob计算S = db*Ha（自己的私钥乘上Alice的公钥）。两边计算的S是相同的。

S = da*Hb = da (db G) = db *(da *G) = db*Hb 等式1

中间人支持到Ha和Hb，无法计算出共享密钥S。即离散对数问题为： <br>
中间人要计算S，必须通过上述 等式1中的一个等式来计算。显然必须知道da或者db，而中间人只知道Ha和Hb，即中间人为了获得da或者db需要从H或Hb中分离出da或db，显然这就是之前所说的离散对数问题。 <br>
现在Alice和Bob得到了共享密钥，后续可以使用共享密钥进行对称加密进行数据传输。通常情况下，点S中x向量被作为共享密钥。
## DTLS
DTLS(Datagram Transport Layer Security)即数据包传输层安全性协议。TLS不能用来保证UDP上传输的数据的安全，因此Datagram TLS试图在现存的TLS协议架构上提出扩展，使之支持UDP，即成为TLS的一个支持数据报传输的版本。

# 3 DTLS
## ECC 概念
## Replay Attacks
重放攻击(Replay Attacks)又称重播攻击、回放攻击，是指攻击者发送一个目的主机已接收过的包，来达到欺骗系统的目的，主要用于身份认证过程，破坏认证的正确性。重放攻击可以由发起者，也可以由拦截并重发该数据的敌方进行。攻击者利用网络监听或者其他方式盗取认证凭据，之后再把它重新发给认证服务器。


# 4 -7 ECC
## ECC 概念 4-5
## 计算 6-7

# 8 加密方法选择条件
# 9-11 Challenges for broadcast security
* scale 10
* dynamic 10  
* low overhead
* package loss
# 12-17 Reliable Broadcast Transmission
## 13 End-to-end approach
## 14 shared key
## 15 Asymetric key: Digital Signature
## 16-17 Trivial broadcast key distribution

# 18 Broadcast Authentication Protocol
k different keys to authenticate every message with k different MAC's
# 19 Hashchain


Job for isc-dhcp-server.service failed because the control process exited with error code.
See "systemctl status isc-dhcp-server.service" and "journalctl -xe" for details.
