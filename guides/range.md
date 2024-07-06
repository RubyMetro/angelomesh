---
layout: page
title: Range and positioning your nodes
---

---
Meshtastic is great because depending on your setup, distances of several miles or more are achievable, but this comes with some considerations on how you position your nodes.

<p class="message">
  Warning: Only place nodes in places where you have PERMISSION to do so. 
</p>
---

## A little bit about LoRa
Meshtastic operates on a frequency that is line of sight, this means that your reception with matter most if there are obstacles between you and the target node, such as trees, houses and buildings, and in the case of San Angelo, terrain. 
---
## Determining line of sight
One place to start with determining if you are going to have line of sight with another node is to use a tool called [ScadaCore.](https://www.scadacore.com/tools/rf-path/rf-line-of-sight/) This will let you place two points on a map and view the elevation map between them, it will also give you a good idea if you have line of sight between these two points. This only takes terrain into account, but that is the biggest obstacle stopping you from getting into contact with another node.
<img src="/Assets/scada.png" width="400"/>

## Positioning your node
If you are still having problems reaching a node, make sure that you are not being blocked by buildings or trees. Sometimes it is hard to tell if there is anything blocking you if it is further away, so what we recommend doing is placing your node up high to reduce the RF shadow cast by trees and buildings. 

## Antennas
One of the biggest factors involving range is the antenna that you are using with your radio. The antennas that come stock with a lot of meshtastic radios are unfortunately pretty inefficient, especially the PCB antennas that come with RAK4631 block modules. The best thing you can do to increase your connectivity in the mesh is to get a different antenna for your radio. When shopping for an antenna make sure to note whether or not it is efficient with or without a ground plane, as most meshtastic radios have only a small ground plane. If you are trying to reach a node that is particularly far away but has access to a larger number of radios, you may also consider a 915mhz yagi to increase your gain. 