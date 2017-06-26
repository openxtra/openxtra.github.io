---
title: "Wireless Network Security vs Wire Based Network Security"
permalink: wireless-vs-wired-network-security.html
author: denis
description: A discussion of wireless network security and how it differs from the security required for a traditional wire based network.
---
One of the hot topics in network management at the moment is how to secure a wireless network. I'm not going to go into depth about wireless security as there are far better sources for that than me. For those interested in an in-depth analysis this [page](http://www.drizzle.com/%7Eaboba/IEEE/) contains a lot of links to appropriate material. Be warned however, it is heavy going!

The main point I want to make in this article is that security on your wire based network is at least as important as your wireless network. Why? A wireless network is considered to be a security threat because people outside your building can, if you're not careful, listen in on your network traffic. True enough so you must be very careful about the security on your wireless segment(s).

If the traffic going over your wireless LAN is not encrypted then people outside your building may be able to read it. Thing is, the same applies to your wire based network too. The tools for capturing packets are a breeze to install and don't take much technical competence to setup (if any) either.

But, what about my switched network. Surely that cures the network visibility problem. Yes it does for most situations, but there are situations where that isn't the case. The switches of old (from not that long ago) were not as secure as they might have been. Many had a hole in their security that meant that if you could flood them with enough new MAC addresses they would stop switching and regress to being a hub. In other words, if I could send out enough packets with new made up MAC addresses, I could then capture all packets passing through my switch.

That's why application level security and encryption is so important. If the conversations between everybody's email client and the email server are encrypted then it doesn't matter too much whether somebody is capturing the traffic (either inside or outside the building). They would be put to considerable inconvenience to decode the encrypted email traffic. I once knew a guy working at a local IT shop. He was the most junior technician in the building. Yet, he knew more about what was going on than anybody else, including the CEO. Why? He was capturing all email traffic going to the email server. Stupid thing is, all it took to cure the problem was clicking a single check box in the Options dialog for Microsoft Outlook on each machine in the building.

There is a lot of hoopla about whether 128 bit encryption is enough or whether it should be 256 bit instead. It is important if you are running a network where the information cannot leak out, for the CIA or military for example. For most shops that isn't as great a constraint. Most companies do not have highly competent hackers sitting outside the building just waiting for a slip up. For everybody else all you really need is a bit of common sense. If it is hard for someone internally to capture sensitive information, then the chances are it will be equally hard for someone outside too.

