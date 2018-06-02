# COMP9337 FINAL QUIZ
## 1. How many data channels are available in Bluetooth Smart, except for device advertisement?
Select one:

a. 37 

b. 39 

c. 38 

d. 40 

37

Physical layer: channels for hopping (40
available channels in 2.4Ghz)
* Advertising: 3 channels
* Data: 37 channels 

## 2. What information in Bluetooth is firstly known to attacker for packet interception without any efforts?
Select one:

a. Channel Hopping Interval 

b. Channel Hopping Increment 

c. Preamble Correct

d. Protocol Data Unit (PDU)

Preamble

Preamble(1 byte)Access|Address(4 bytes)|PDU(2 to 39 bytes)|CRC(3 bytes)

## 3. How does a RADIUS server communicate with an authenticator? 
a. UDP ports 1812 and 1813 Correct

b. Encrypted IPsec tunnel 

c. TCP ports 1645 and 1646 

d. Encrypted TLS tunnel 
UDP ports 1812 and 1813
## 4. A Security Policy Database
a. contains rules how security mechanisms are applied in a given system, e.g. the kernel using TLS 

b. is commonly implemented in Oracle SQL 

c. contains rules how the assets of an organisation must be insured to protect against losses 

d. contains rules how IPsec must be applied to incoming and outgoing packets Correct

contains rules how IPsec must be applied to incoming and outgoing packets
## 5.What is the maximum number of active Bluetooth devices in a piconet？
Select one:


a. 7 

b. 9 

c. 8 Correct

d. 10 

8
## 6.Which algorithm is used to encrypt the Protocol Data Unit (PDU) in bluetooth
a. RSA 

b. Ecliptic Curve Cryptography 

c. HMAC 

d. AES-CCM Correct

AES-CCM
## 7.In epidemic propagation model Nodes can request data from which of the following：
Select one:


a. from its nearest neighbours caching the data 

b. from cloud resident remotely in the Internet Incorrect

c. All of the other choices 

d. the source of the information (e.g. a base station) 

from its nearest neighbours caching the data
## 8. Which of the following is true for a Merkle Tree:
Select one or more:


a. Values can be revealed in any order. 

b. A user has choice to pre-configure revelation either sequentially or in any order 

c. Values can be revealed only sequentially. Incorrect

Values can be revealed in any order.

Merkle-trees: allowing for the pre-authentication of a set of values with a single digital signature(on the root u0 of the tree) and for the revelation of those values in any order

## 9.A Security Association...
Select one:


a. describes either AH or ESP settings for a simplex connection Correct

b. describes both AH and ESP settings for a duplex connection 

c. is a multinational organisation in charge of security standards 

d. describes both AH and ESP settings for a simplex connection 

describes either AH or ESP settings for a simplex connection


A Security Association (SA) is the establishment of shared security attributes between two network entities to support secure communication. An SA may include attributes such as: cryptographic algorithm and mode; traffic encryption key; and parameters for the network data to be passed over the connection. The framework for establishing security associations is provided by the Internet Security Association and Key Management Protocol (ISAKMP). Protocols such as Internet Key Exchange and Kerberized Internet Negotiation of Keys provide authenticated keying material.[1]

An SA is a simplex (one-way channel) and logical connection which endorses and provides a secure data connection between the network devices. The fundamental requirement of an SA arrives when the two entities communicate over more than one channel. Take, for example, a mobile subscriber and a base station. The subscriber may subscribe itself to more than one service. Therefore, each service may have different service primitives, such as a data encryption algorithm, public key, or initialization vector. To make things easier, all of this security information is grouped logically, and the logical group itself is a Security Association. Each SA has its own ID called SAID. So both the base station and mobile subscriber will share the SAID, and they will derive all the security parameters.

In other words, an SA is a logical group of security parameters that enable the sharing of information to another entity.

## 10. Which of the following variable is not used during the 4 - Way Handshake to produce a pairwise transient key (PTK)?
Select one:


a. Pairwise Master Key 

b. Group Master Key 

c. Authenticator MAC address 

d. Nonces Incorrect

The correct answer is: Group Master Key


PTK-Pairwise Transient Key: A value derived from PMK, Authenicator nonce(Anonce), Supplicant nonce(Snonce), Authenticator Address, Supplicant Address. This is used to encrypt all unicast transmission between client & an AP. PTK consist of 5 different keys. They are:

1. KCK - Key Confirmation Key used to provide data integrity during 4 -Way Handshake & Group Key Handshake.

2. KEK – Key Encryption Key used by EAPOL-Key frames to provide data privacy during 4-Way Handshake & Group Key Handshake.

3. Temporal Key – used to encrypt & decrypt MSDU of 802.11 data frames between supplicant & authenticator

4. Temporal MIC-1

5. Temporal MIC-2

And also, my lecture slides says:

PTK = HMAC_SHA_1(PMK || AP_nonce || STAnonce || AP_MACaddr || STA_MACaddr)

Now my question is, how can I actually calculate PTK if following keys are given?

KCK = "aaaaaaaaaaaaaaaa"

KEK = "bbbbbbbbbbbbbbbb"

TK = "cccccccccccccccc"

## 11.Which of the following is correct:
Select one:


a. TLS runs above IPsec, which runs above IP 

b. TLS runs above IP, which runs above IPsec 

c. TLS runs on the application layer 

d. TLS can be used together with IPsec Correct

TLS can be used together with IPsec 

https://security.stackexchange.com/questions/42990/which-is-better-for-server-to-server-communication-ipsec-or-tls?utm_medium=organic&utm_source=google_rich_qa&utm_campaign=google_rich_qa

## 12.The authentication server used in conjunction with 802.1X employs such things as

Select one:


a. All of the other choice 

b. RADIUS Incorrect

c. Active Directory 

d. LDAP 

a. All of the other choice 

b. RADIUS 

c. Active Directory 

d. LDAP 

All of the other choice

## ? 13. IPsec

Select one:


a. is more secure than TLS because it uses X.509 

b. is activated on-demand when an applications requires it Incorrect

c. is more secure than TLS because it does not use X.509 

d. requires administrative effort as it runs in kernel space 

The correct answer is: requires administrative effort as it runs in kernel space

https://security.stackexchange.com/questions/42990/which-is-better-for-server-to-server-communication-ipsec-or-tls?utm_medium=organic&utm_source=google_rich_qa&utm_campaign=google_rich_qa

## 14. When a new client is connected to an authenticator using the 802.1X protocol, the authenticator's port is enabled and set to the “authorized” state.
Select one:

a. True 

b. False Correct

False.

Unauthorized

## 15.Select the right key combination from the following that is broadcast and multicast 802.11 frames in 802.11 Enterprise security
Select one:

a. Pairwise Master, Group Temporal 

b. Group Master, Group Temporal 

c. Pairwise Transient, Group Temporal 

d. Master Session, Pairwise Transient Incorrect

Pairwise Transient, Group Temporal

## 16.Which of the following best characterizes a Sybil attack:
Select one:

a. A node presents several identities to break fault tolerance or reputation systems Correct

b. All of the other choices 

c. A Sybil server is created in the cloud to capture packets for passive analysis 

d. A new node is introduced in the network to launch MiTM 

a. A node presents several identities to break fault tolerance or reputation systems Correct

(one node presents several identities to defeat fault tolerance)

Wormhole Attack(fake nonexisting links)

## 17.Comparing IPsec to TLS, which statement is true:
Select one:

a. IPsec may have better performance if no TCP is used 

b. IPsec is more secure because it uses RSA and TLS does not 

c. None of the choices are true Incorrect

d. TLS is more secure than IPsec because it uses Diffie-Hellman key exchanges 

The correct answer is: IPsec may have better performance if no TCP is used

 Internet Key Exchange (IKE, sometimes IKEv1 or IKEv2, depending on version) is the protocol used to set up a security association (SA) in the IPsec protocol suite. 

Why does IKE use UDP instead of TCP?
https://networkengineering.stackexchange.com/questions/29669/why-does-ike-use-udp-instead-of-tcp
## 18.Which of the following is true Signature Based Attack:

Select one:

a. Attacker fools a node and obtains the key used to generate the signature 

b. Attacker keeps sending forged data to deplete Node’s energy in performing signature verification Correct

c. A user’s signature is forged to access the system. 

d. Attacker keeps sending forged data to since one of them would eventually succeed 

Attacker keeps sending forged data to deplete Node’s energy in performing signature verification

## 19. Which Layer 2 protocol is used for authentication in an 802.1X framework?

Which Layer 2 protocol is used for authentication in an 802.1X framework?


Select one:

a. EAP Correct

b. MS - CHAPv2 

c. CHAP 

d. PAP 

EAP

* MS - CHAPv2: MS-CHAP is the Microsoft version of the Challenge-Handshake Authentication Protocol, CHAP. 
MS-CHAP is used as one authentication option in Microsoft's implementation of the PPTP protocol for virtual private networks. It is also used as an authentication option with RADIUS[2] servers which are used with IEEE 802.1X (e.g., WiFi security using the WPA-Enterprise protocol). It is further used as the main authentication option of the Protected Extensible Authentication Protocol (PEAP).


* CHAP:  the Challenge-Handshake Authentication Protocol (CHAP) authenticates a user or network host to an authenticating entity. That entity may be, for example, an Internet service provider. CHAP is specified in RFC 1994.

CHAP provides protection against replay attacks by the peer through the use of an incrementally changing identifier and of a variable challenge-value. CHAP requires that both the client and server know the plaintext of the secret, although it is never sent over the network. Thus, CHAP provides better security as compared to Password Authentication Protocol (PAP) which is vulnerable for both these reasons. The MS-CHAP variant does not require either peer to know the plaintext and does not transmit it, but has been broken.[1]
* PAP :Password Authentication Protocol (PAP) is a password-based authentication protocol used by Point to Point Protocol (PPP) to validate users. Almost all network operating system remote servers support PAP.

PAP is considered a weak authentication scheme (weak schemes are simple and have lighter computational overhead but are much more vulnerable to attack; while weak schemes may have limited application in some constrained environments, they are avoided in general). Among PAP's deficiencies is the fact that it transmits unencrypted passwords over the network. PAP is therefore used only as a last resort when the remote server does not support a stronger scheme such as CHAP or EAP.
## ?20. In the D-H key exchange protocol, D-H may be used over ECC.
Select one:

a. True 

b. False Incorrect

True

https://crypto.stackexchange.com/questions/37200/how-does-dh-work-when-combined-with-ecc-or-rsa?utm_medium=organic&utm_source=google_rich_qa&utm_campaign=google_rich_qa

## 21. What is the difference between the inner and outer identity in EAP Tunnelled methods?
Select one:

a. The inner identity is only for authentication server credentials provided to the supplicant. Incorrect

b. The outer identity is in plain text; the inner identity is securely transmitted inside a TLS tunnel. 

c. Only the authentication server provides its credentials in the outer identity response. 

d. The inner identity must correspond to the outer identity for realm – based authentications. 

The correct answer is: The outer identity is in plain text; the inner identity is securely transmitted inside a TLS tunnel.

## 22. What type of information is used by the authenticator and authentication server to validate each other?

Select one:


a. Username and password 

b. Client-side X.509 digital certificate 

c. Shared secret Correct

d. Server-side X.509 digital certificate 

Shared secret

## 23.
Which of the following characterizes the wormhole the attack best:

Select one:


a. An attacker creates a worm and floods the network Incorrect

b. A hole is created in user’s disk to destroy the data 

c. An attacker records packets at one location in the network, tunnels them to another location. 

d. A worm is created and launched via the Internet 


An attacker records packets at one location in the network, tunnels them to another location.