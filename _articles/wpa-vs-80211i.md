---
title: "WPA vs WPA2 (802.11i): How your Choice Affects your Wireless Network Security"
permalink: wpa-vs-80211i.html
layout: page
description: A discussion of why 802.11i (WPA2) provides stronger wireless security than WiFi Protected Access (WPA) and WEP, why there is a need for a new standard and why you should use it.
---
WPA has, rightly, been admired as a masterpiece of retro engineering. It addresses the weaknesses of WEP and the result is a very secure security system that is backwardly compatible with most existing WiFi compliant equipment. WPA is a practical solution that will provide more than adequate security for most wireless network applications.

However WPA is in the end a compromise solution. It still relies on the RC4 encryption algorithm and TKIP (Temporary Key Integrity Protocol). Although unlikely, the possibility of new weaknesses being discovered still exists.

A completely new security system, avoiding the design flaws of WEP entirely, represents the best long term, scalable solution to wireless LAN security. To this end the standards committee decided to design a new security system from the ground up. This is the new 802.11i standard, also known as WPA2 by the [WiFi Alliance](http://www.wi-fi.org/).

## What is 802.11i?

802.11i uses the concept of a Robust Security Network (RSN). In RSN wireless devices need to support additional capabilities. This requires new hardware and software drivers making a fully compliant RSN network incompatible with existing WEP equipment. In the transitional period both RSN and WEP equipment will be supported, (in fact WPA/TKIP was a solution designed to make use of older equipment) but in the longer term WEP devices will be phased out.

802.11i allows for various network implementations and can use TKIP, but by default RSN uses AES (Advanced Encryption Standard) and CCMP (Counter Mode CBC MAC Protocol) and it is this which provides for a stronger, scalable solution.

## What is AES/CCMP?

Advanced Encryption Standard (AES) is the cipher system used by RSN. It is the equivalent of the RC4 algorithm used by WPA. However the encryption mechanism is much more complex and does not suffer from the problems associated with WEP. AES is a block cipher, operating on blocks of data 128bits long.

CCMP is the security protocol used by AES. It is the equivalent of TKIP in WPA. CCMP computes a Message Integrity Check (MIC) using the well known, and proven, Cipher Block Chaining Message Authentication Code (CBC-MAC) method. Changing even one bit in a message produces a totally different result.

One of the worst aspects of WEP was the management of the secret keys. Many administrators found it impractical to manage keys in larger networks. As a result WEP keys were often not changed making it easier for hackers.

RSN defines a hierarchy of limited life keys, similar to TKIP. AES/CCMP requires 512bits to accommodate all the keys, less than TKIP.

Also like TKIP master keys are not used directly, but are used to derive other keys. Fortunately the administrator only needs to provide a single master key.

Messages are encrypted using a secret key (128bits) and a 128bit block of data. The encryption process is complex, but again the administrator does not need to be aware of the intricacies of the computations. The end result is encryption that is much harder to break than even WPA.

## Conclusion

802.11i is by far the strongest security system for wireless networks. The purist would argue that anything less is the equivalent of no security at all.

When the 802.11i standard is ratified RSN (WPA2) compatible equipment will begin to appear. 802.11i (WPA2) will be the most robust, scalable, and secure solution and will appeal particularly to enterprise users where key management and administration has been a major headache.

802.11i has been designed using proven technologies. Security has been designed from scratch in full consultation with the best cryptographers and stands every chance of being the solution that wireless networks need. Although no security system can ever be considered totally unbreakable, 802.11i security is a dependable solution and seems unlikely to be breached. It suffers none of the problems of older systems.

802.11i is a wireless security system that you can depend on. You can use WPA to accommodate older equipment and as that reaches the end of its useful life you can upgrade to a fully compliant RSN network.

