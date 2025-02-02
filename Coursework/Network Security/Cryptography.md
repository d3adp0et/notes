# Cryptography

- Read Introduction to Modern Cryptography: Principles and Protocols (Jonathan Katz, Yehuda Lindell, second edition, Chapman & Hall/CRC)
- crypto building blocks:
	- encryption (symmetric and asymmetric)
	- hashing
	- message authentication code
	- authentication code
	- digital signature functions
	- cryptographic random numbers generation
- ns service:
	- CIA
	- access-control
	- non repudiation
	- availability
	- key management
	- audit

## Informal Security Attack
- Kent's classification
	- passive attacks (changes nothing just observes)
	- active attacks (modifies or remove data or do any kind of change that causes harm)
- Security attacks
	- interception
	- interruption
	- modification
	- fabrication

- Dolev-Yao Model

- **Kerchoff's principle** "no security by obscurity"
	- the cipher should be secure even if the intruder know everything about the encryption process(except for the secret key)
	- basically only thing you defend at the end is the **"key"**

- Security in every layer of protocol stack (helps hide more)     
	- application layer : telnet/ftp(ssh), http/https, mail(PGP)
	- transport layer : SSL/TLS
	- network layer : IPsec,IKE
	- link layer : IEEE802.1x/IEEE802.10, WPA
	- physical layer : spread-Spectrum, quantum crypto, etc

- Block vs Stream Ciphers:
	- block:
		- input: block of n bits
		- output: block of n bits
		- eg: AES
	- stream:
		- input: stream of symbols
		- output: stream of symbols
		- eg: GSM, SNOW 3G
- Asymmetric and Symmetric
