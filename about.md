---
layout: page
title: About
---
---
This site is dedicated to providing information to the general public about San Angelo's growing network of [Meshtastic](https://meshtastic.org) nodes, used for decentralized text message communication, as well as provide instructions for connecting to the mesh and guides for building your own nodes.

## about meshtastic
Meshtastic is a firmware package that allows radios to communicate with each other over the ISM band (in the United States, this is on 900mhz.) It also allows for these radios to act as repeaters and pass traffic to other radios, forming a mesh network. Messages sent over the network have the option of being encrypted and channels can be made so that you have private communication with multiple people. Meshtastic is able to achieve high range with LoRa, which is a modulation technique that works below the noise floor, also allowing these radios to consume very little power and last for days on batteries as low as 1100mAh (or even lower!) 

A good resource to learn more about Meshtastic and LoRa is to look at the presentation files from the San Angelo Amateur Radio Club meeting about Meshtastic [here,](https://www.w5qx.org/2024/01/11/lora-presentation-files/) which contains links to learning resources.

## about San Angelo's mesh network
currently there are a few dozen nodes spread around san angelo, most of which are in the southern region near Lake Nasworthy and San Angelo's ragional airport. We are trying to expand our coverage into town and downtown, where more nodes are needed due to terrain and building density. A great way to get involved is to join the [Discord](https://discord.gg/Kw53pzwyuQ), or to get involved in the [local amateur radio club,](https://w5qx.org) as many of our members are also involved in San Angelo's mesh network.

## Well that's great and all, but why?

1. It is decentralized and open to everyone. Because this mesh network does not rely on any one server or repeater, communication on the network is available to everyone who decides to use it. This also means that the network remains resilient when one or two nodes go offline, because other nodes can pick up the added load, as opposed to centralized infrastructure.

2. Emergency communications. Many of you that lived through the 2021 winter storm here in texas will understand that being able to communicate with others and get help when infrastructure is down is crucial during an emergency. Because a lot of our nodes are powered through solar or long lasting batteries, the mesh network remains online when all else fails, allowing the community to coordinate and plan.

3. Privacy. When you send a message through an encrypted channel on the mesh network, you have all of the same benefits of being able to use other radios to bounce your message to your destination while knowing that no person or entity is secretly reading your traffic.

4. Telemetry. The mesh network has other use cases that dont involve communication with people. Meshtastic can be used with other software or sensors to deliver information across the network. One example of this is ATAK, which can be used with meshtastic for decentralized geospatial and situational awareness.

5. No license required. Because meshtastic operates on the ISM band, anyone can use it, and you do not need to have an amateur radio license to transmit. This is also what makes meshtastic private.

This website was built with [Jekyll](jekyllrb.com) and is hosted on [Github Pages.](https://pages.github.com) Made using the [Hyde](https://github.com/poole/hyde) theme. You can look at the source code for this website [here.](https://github.com/rubymetro/angelomesh) Hyde is released under the [MIT License,](https://en.wikipedia.org/wiki/MIT_License) which has also been attached to the source code of this website.

<p xmlns:cc="http://creativecommons.org/ns#" xmlns:dct="http://purl.org/dc/terms/">The content on this website, written by <span property="cc:attributionName">Christian Thompson,</span> is licensed under <a href="https://creativecommons.org/licenses/by-nc-sa/4.0/?ref=chooser-v1" target="_blank" rel="license noopener noreferrer" style="display:inline-block;">CC BY-NC-SA 4.0</a></p>