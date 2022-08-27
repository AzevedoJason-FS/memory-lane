---
title: JSON Web Token (jwt)
description: JSON Web Token Talk
layout: singlePost
---

![My helpful screenshot](/memory-lane/images/jwt_logo.png)

So you may ask yourself, what in the world is a **JSON Web Token**? Well as you could guess it is quite literally what the name defines. It is a self-contained way for securely transmitting information between parties as a JSON object. First it is important to understand the basic structure of a **JSON Web Token**; It consists of thre seperate parts:
- Header
- Payload
- Signature
A typical token would look like this (xxxxx.34ddda.aaaaaa) Hence the periods (.) within the token seperating all three parts.

**Header**
The header typically consists of two parts: the type of the token, which is JWT, and the signing algorithm being used, such as HMAC SHA256 

**Payload**
This part typically contains the claims, which is different information regarding the user.

**Signature**
Lastly we have the signature. This is a secrete 'key' that the developer may have that is used to verify the message wasn't changed along the way. It is added to the end of the Header + Payload
