---
template: blog-post
title: What is TLS, and how does it work?
slug: about-tls
date: 2021-03-07 20:17
description: An article about TLS, how it works, and its importance.
featuredImage: /assets/141dafbf083ce49515283c071b576a3f.png
---


                TLS or Transport Layer Security is a security protocol used in the protection of web traffic. Being a continuation of SSL, TSL is very important in our everyday lives. The first release of TSL was actually patch 3.1 of SSL, but the name of the protocol was changed to show that the project was no longer associated with Netscape. TSL is used to encrypt web traffic between a user and server. The protocol does this through three main components. Encryption, hiding the data from people who aren’t supposed to see it. Authentication, ensures the identity of the people exchanging information. And Integrity, making sure that the data sent does not get altered or tampered with. Websites that don’t use TLS are open to packet sniffing and man in the middle attacks, where your data is intercepted in transit. This could lead to data being switched with malware or a password you enter being stolen. Without TLS none of our web traffic would be kept secret and would be open to the public. TLS is implemented in many applications to protect web traffic. The most well known of these applications is Google Chrome.

                TLS works through TLS Certificates and the TLS handshake. The TLS Certificate is issued to a domain by a Certificate Authority, like cloud flare. These certificates contain information about the web server, the owning party and the server’s public key. The certificate is used in the TLS handshake to authenticate the server’s identity. The TLS handshake is how a connection is initially made between two systems that are using TLS. This starts off with the two systems communicating on which version of TLS must be used for the connection. After this a cipher suite is decided on that will be used for the session keys. Then the server’s TLS certificate is verified and finally the session keys are generated. The connection between the systems is established and ready for protected traffic.

                The TLS session keys are the entire point of the TLS protocol. These session keys allow for asymmetric encryption of the data that is being sent, and are protected as to not be leaked. Asymmetric encryption is also not anywhere near as efficient as symmetric encryption and TLS uses a combination of the two to improve performance of the algorithms.

                The difference between symmetric encryption and asymmetric encryption is that asymmetric encryption works in one direction. With symmetric encryption the encryption works both ways, using the same key. This can be exemplified using 8 bit binary numbers:

```
		1 0 1 0 1 1 0 1 – Encryption Key		1 0 1 1 1 0 0 1 – Data for Encryption
					1 0 1 0 1 1 0 1 – Encryption Key
					1 0 1 1 1 0 0 1 – Data for Encryption

					0 0 0 1 0 1 0 0 – Encrypted Data

					0 0 0 1 0 1 0 0 – Encrypted Data
					1 0 1 0 1 1 0 1 – Encryption key
					
					1 0 1 1 1 0 0 1 – Decrypted Data
```

                The above example uses the exclusive or to exemplify symmetric encryption. Taking the encryption key and the data to be encrypted, we get the encrypted data by evaluating the exclusive or for the matching bits, a 1 and a 0 is a 1 and a 1 and a 1 is a 0. This gives the data in an encrypted form that can be decrypted by performing the same exclusive or operation with the encrypted data and encryption key. An example of a functions that completes this coded in javascript is below:

```
const encryptData = (encryptKey, data) => {
    let encryptedData ='';
    if(encryptKey.length === data.length)
    {
        for(let i = 0; i < encryptKey.length; i++)
        {
            if((encryptKey[i] === '1' || data[i] === '1') && encryptKey[i] !== data[i])
            {
                encryptedData = encryptedData.concat('1');
            }
            else
            {
                encryptedData = encryptedData.concat('0');
            }
        }
    }
    console.log(encryptedData);
}
```



                The session keys come in the form of a private and public key for both the systems in the connection. An example for this is a user and a web app. In this case the user encrypts a message with their private key and sends it to the web app that has the public key to decrypt the message. This encryption only works in one direction and due to that fact, the sending user is verified. The last part of TLS is the message authentication code that is included to ensure that the data is not changed.

                Without TLS the Internet would be a more dangerous place for our data. This is why when browsing make sure that you are browsing websites with https://.