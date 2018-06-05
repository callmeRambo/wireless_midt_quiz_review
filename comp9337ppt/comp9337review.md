# 9337 review (Module 2-3)
# MOD 2
# 1. Encryption and Decryption
## Security Fundamentals
1. confidentiality:
only sender, intended receiver should “understand” message
contents
2. authentication:
sender, receiver want to confirm identity of each other
3. message integrity:
ensure message not altered (in transit, or afterwards)
without detection
4. Non-repudiation:
associating actions or changes to a unique individual

## Public Key Cryptography(RSA)
message-->alice encrypt with bob's pub key(K+) --> bob decrypt with bob's pri key(K-(K+))

## Symmetric Key Cryptography(Fast)
mess --> alice with key --> bob with same key

## Hash/Message Digests (MD) For integrity check
    hash function For comparison not for encryption
mess --> hash func --> H(m)

## HMAC
Keyed-hash message authentication code:

a message authentication code that uses a cryptographic key in
conjunction with a hash function
## HMAC: Integrity and Authentication

    1.ALICE SEND mess combine with (hashed mess and shared secret, which is called HMAC)
    2.BOB hashed mess and shared secret, check with HMAC.
## Digital signatures
cryptographic technique analogous to hand-written
signatures

Bob signs m by encrypting with his private key KB,
creating “signed” message, KB(m)

bob send mess --> public key encrypt message and bob's private key encrypt message --> alice veryfy with bob's public key and check if former and later same.
# 2.Symetric Ciphers
## Block Cipher
1-to -1 mapping is used to map k 1 mapping is used to map k bit blocks of cipher.

1. cipher block chain
recall des cbc.

## DES and AES
2. electionic codebook ECB
SPLIT into blocks and encrypt each one

## 3. WEP AND WPA
1. WEP security hole: 24 bit IV
WEP approach: initialize WEP approach: initialize  keystreamkeystream with key + new IV for with key + new IV  for each packet
2. ENCTRYPTION
IV + KEYID + (DATA + ICV) ENCRYPTED
3. DECRYPTION
RANDOM GENERATOR(IV + KEY) XOR DATA and check with ICV

## 4. WPA

# MOD3
## RSA
1. 加密
    明文^E MOD N 
    公钥是（E,N)
2. 解密
    密文^D MOD N
    私钥（D,N)
3. 求公钥私钥过程
https://blog.csdn.net/dbs1215/article/details/48953589
```
求N
求L（L为中间过程的中间数）
求E
求D
```
1. ## N
    准备两个质数p，q。这两个数不能太小，太小则会容易破解，将p乘以q就是N
2. ## L 最小公倍数
    L=lcm（p－1，q－1）
3. ## E
    E必须满足两个条件：E是一个比1大比L小的数，E和L的最大公约数为1 

    用gcd(X,Y)来表示X，Y的最大公约数则E条件如下：
    
    1 < E < L

    gcd（E，L）=1
4. ### D
    1 < D < L

    E*D mod L ＝ 1

## SSL : Secure Sockets Layer

