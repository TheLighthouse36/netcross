# Netcode Notes
This document will contain all my notes about netcode and related information

## Terms and Definitions
- Ping (Round trip time): The time between ICMP Echo Request and Reply usually measured in ms
- Lag: The time between the client and server (the desync)
- Routing: how data chooses the fastest route between you and the server
- Update Rates: The time between when data is sent, The higher the less the additonal delay and for better online experiences
- Tick/Simulation rate: How often the game processes data
- Packet Loss: Data Packets are guranteed to reach destination, 
- client side server authorization: client registers, server authorizes
- Server side authorization: only server perspective matters

## Lag compensation
- Disconnect high ping players (usually a bad solution)
- using multiple authorization methods depending on ping thresholds

## Network Models
- Dedicated Server <- best overall option
- Client As Host
- Peer to Peer

## Resource and links
- Netcode 101