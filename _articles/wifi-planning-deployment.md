---
title: Wireless Network Planning and Deployment
permalink: wifi-planning-deployment.html
description: Planning a WiFi (wireless) network is similar in many respects to planning a wired network. You have to consider all the basics, how many users do you need to accommodate, where are you going to deploy the solution and so on. But wireless also brings with its own set issues, chief amongst these is the common perception that WiFi is insecure.
---
This document attempts to explain how you should go about building a wireless LAN, the issues involved and the areas that you should be concerned about.

WiFi LANs will improve your business. Research has shown that your users will stay connected longer and work more efficiently, that wireless is more flexible than wired systems, and that users benefit from the increased ease of use of wireless. The network is easier and cheaper to install than a wired system, and you can accommodate the latest mobile technologies, PDAs and Laptops.

It is assumed throughout this document that you will be operating the WiFi LAN in Infrastructure mode, which is normal for enterprise networks.

## Plan a Pilot Scheme

If you haven’t already done so, check to see whether you already have a wireless network. With Wireless Access Points (WAP) so cheap somebody may have already installed an unofficial wireless network already. Or, perhaps they might be using the ad-hoc abilities of all WiFi network cards. Before you start a pilot scheme you need to know what you already have. It is like having a survey done on a building site before proceeding with construction.

The sensible way to proceed is to start small with a view to expanding the system when tangible business benefits can be demonstrated. Think about who will benefit most from having a wireless network. Itinerant workers, like sales people are a logical first step. Places like conference rooms are also a good place to start.

### Scope

Define the scope of the pilot scheme. It is important that the pilot is a truly representative sample of your network. The scale and coverage must be sufficient so that the results they will be realistic on a larger scale. The number and types of users should be a representative cross section.

### Locations

Typically sales offices, executive rooms, and new buildings as yet not wired to the network, represent good sites for the pilot, but you should try to include as many departments and job types as possible to determine how the different parts of your organization use the wireless network and how they derive added value from it.

### Zones of Coverage

Enterprise WiFi LANs use hardware devices known as Access Points. Access Points need to be attached to the wired network. You would be well advised to perform a site survey to ascertain exactly where the cable runs are. You will want to allow coverage of conference rooms, office suites, production facilities, warehouses or whatever is appropriate in your circumstances, while at the same time minimizing any disruption or reconfiguration of the wired network, now or when you expand the WiFi network later.

Each Access Point has a limited range, particularly if there are walls or floors between devices and the Access Points. Ranges quited are typically 50metres in enclosed offices, and up to 300metres in open spaces. Your site survey will show you where best to deploy the Access Points for maximum coverage.

### Return On Investment (ROI)

It may not be easy to calculate the ROI but it a crucial metric for justifying the expansion of the WiFi LAN. If you can prove that productivity has increased and that real value has accrued to the business then the pilot will have been a success. One measure is time spent on the LAN. A recent survey showed that wireless users spent on average 3.75 hours longer on the network and productivity increased by 27%. You should give some thought to other such measures of benefit to the organization.

Make sure that you support team are up to speed on the new technology, that they know the issues that may arise, and that your users are prepared for the new ways of working that wireless allows. Happy users are a sure way to a successful pilot scheme.

## Decide on a Security Policy

The one thing that most people know about WiFi networks is that they are insecure. Is this reputation justified?

Wireless is unlike other LAN technologies. A wired system is fairly secure because the only way to join the network is by physically attaching a device. Wireless signals broadcast everywhere and anyone within range can see that traffic and attempt to join the network. This brings with it security, authentication and privacy issues. WiFi has security built in and you should use as many of these features as possible even though several much publicized weaknesses have been revealed. The fact is that any security is better than none and breaking into a WiFi network requires knowledge, determination and time.

### SSIDs

The network will need an SSID (Service Set Identifier) so that users can have access. Basically this is a name for the network segment and a way or grouping clients and Access Points. The SSID must be the same for all clients and Access Points in a group. You can, of course subdivide your network using different SSIDs.

Do not use the manufacturer default SSID, and do not use anything too obvious like your company name (amazingly most networks do). Switch off the broadcasting of the SSID in the Access Points.

It is worth bearing in mind that SSIDs can in no way be considered secure. It is possible for wireless cards to connect to any SSID and whatever you set can be easily detected by using a packet sniffer. However there is no value in making it embarrassingly easy for a hacker to guess who’s network it is.

### Basic Security

Some Access Points allow MAC Filtering, basically a list of acceptable MAC addresses are configured into the Access Point and it will not allow access to any addresses not in the list. If your devices support this use it, but bear in mind that it is not difficult to mimic MAC addresses and if a device is lost or stolen its address will have to be removed from all the relevant Access Points.

Also be aware that wireless cards can operate in Ad-hoc mode, allowing direct connections between devices without the need for Access Points. Although very convenient it is exceedingly insecure. Forbidding its use is wise but a very difficult policy to enforce.

### WEP

Wired Equivalent Privacy. The encryption system defined in the 802.11 standard. Available in two levels, 64bit and 128bit. Unfortunately WEP has some serious flaws that mean it can be defeated and so it has developed a reputation for being insecure.

In practical terms WEP will protect you from casual attacks and only a determined hacker with time and skill will be able to break your keys. You should always use 128bit encryption if possible.

The attacks on WEP depend on the hacker capturing a number of packets which include a so-called Weak IV (Initialization Vector). Many newer systems never send Weak IVs and so hackers have no practical method for cracking the encryption. Even if you do send Weak IVs the hacker needs to capture enormous numbers of packets, often several million to begin attempting to crack the encryption. It may take several days or weeks to capture enough packets.

Change your WEP keys frequently. This can be an administrative chore but it means that a hacker has to start all over again. For your pilot scheme the administration may be not be too much of a problem. However, it must be admitted that the administration of keys is not good in WEP. If you are planning a large network you may find some of the advanced security systems easier to administer.

### Advanced Security

It makes sense to use the best security you can get hold of. 802.11x is a security system that features device authentication and dynamic session keys. It is stronger than WEP and should be implemented if you have it. Bear in mind though that it requires the use of a RADIUS Server (Remote Authentication Dial-In Service) on the wired network, again with performance and increased cost penalties.

WPA (WiFi Protected Access) is an interim security standard implemented by the WiFi Alliance, an Industry body that ensures compatibility of equipment. WPA incorporates the benefits of 802.11x and also addresses the issues with WEP by using a more advanced system of keys known as TKIP (Temporal Key Integrity Protocol).

EAP (Extensible Authentication Protocol) allows multiple authentication methods. The exact details vary with the Operating System being used.

If none of the above are secure enough then you should consider using one of the proprietary systems available, such as Cisco’s LEAP (Light Extensible Authentication Protocol). One major consideration is that such systems limit your choice of equipment since most are tied to a particular manufacturer. Also bear in mind that these cost a lot of money and may impact performance.

VPN (Virtual Private Network) technology is available from many manufacturers and may also be an alternative worth considering, again this may be a costly option.

The 802.11 standards are being improved and (eventually) 802.11i will provide a Robust Security Network (RSN), the drawback being that new hardware and software will be required to operate a fully compliant RSN network.

### What Types of Threat are there?

Apart from weaknesses in encryption, hackers can attempt to exploit other aspects of wireless operation.

### Denial of Service Attacks

Hackers may attempt to disrupt your network by swamping your Access Points with packets asking to be Authenticated or by simply overloading the AP, or by generating lots of radio noise. These are known as Denial of Service attacks.

### Intrusion

Hackers may attempt to install Rogue APs or Rogue Clients so that they can intercept traffic to legitimate users. It is important that you audit your APs and Clients frequently to check for rogue devices.

There a number of software tools freely available on the Internet that allow hackers to attempt to break into your network. AirJack for example generates management traffic and can be used for a range of attacks.

Devices such as the Neutrino Intrusion Detection System will Alert you to all of the above types of attack as well as logging ands reporting operational parameters.

## Install the Network

Decide on the equipment to use and order it in plenty of time.

You will need to build the Infrastructure first using suitable Access Points. If your buildings are metal framed or if there are obstructions you may find it useful to source equipment that allows various antenna options. In this way you will be able to fine tune the reception areas.

Some equipment supports Power over Ethernet (802.3af), which may be useful if electrical supply points are difficult to provide.

Equip your Clients with suitable wireless network cards. Install the software drivers in all the Client devices. Usually the manufacturers installation software is sufficient, but you may have to create customized installations for your users.

## Train your Users

The success of your pilot scheme depends on your users understanding their new systems and getting value from the new network. You need to ensure that they receive sufficient training and that they will make use of your support system.

You will use the support system to gather use feedback. Remember that you need to know about more than just technical problems. You also need to gather data about how long users stay on the network, how their working patterns have been change, if they are working more efficiently, and so on. Armed with this information you will be able to perform a realistic ROI calculation.

## Evaluate the Results of your Pilot Scheme

When your pilot scheme has run its course make your reports, calculate the ROI, decide on ways that things might be improved. Try to anticipate what might be different in a larger network.

## Scale the Scheme if Appropriate

If you decide to expand the wireless network go through the planning process again. You will need to ensure that your basic assumptions are applicable to the new wider context.

Pay particular attention to where you want the new wireless zones to extend to, and double check that the security measures you have employed are scalable to a larger network. For example, administration of WEP keys can be a nightmare on larger systems, consider using WPA instead.

Installing a wireless LAN has the potential to save you money, increase productivity, and bring many benefits to your business and users. Careful planning and deployment will enable you to maximize these benefits.