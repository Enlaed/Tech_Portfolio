# Lab 01 — Observing Basic Network Communication

## Overview

As part of my early exploration into technology, I have been studying how devices communicate across networks. While learning the theoretical concepts behind the TCP/IP model, I wanted to move beyond reading and actually observe how communication happens between devices.

This small lab experiment was designed to help me visualize basic network communication in a controlled environment.

The goal was simple: build a minimal network and observe how one device verifies connectivity with another.

---

## Tools Used

- **Cisco Packet Tracer** – to build and simulate the network environment  
- **Command Line (Ping Utility)** – to test connectivity between devices  

---

## Lab Environment

The network was intentionally kept simple to clearly observe the communication process.

Devices used:

- 1 Personal Computer (Client)
- 1 Server
- 1 Switch

Topology:

All devices were configured within the same Local Area Network (LAN).

---

## Experiment

After configuring the devices and assigning IP addresses, I used the **ping command** to test communication between the PC and the server.

Using **Packet Tracer’s Simulation Mode**, I observed the packet flow that occurred when the ping command was executed.

This made it possible to see the sequence of events that allows two devices on the same network to communicate.

---

## Key Observations

During the simulation, I observed that:

- The PC first performs an **ARP broadcast** to identify the destination device’s MAC address.
- Once the address is resolved, the PC sends an **ICMP Echo Request**.
- The server responds with an **ICMP Echo Reply**, confirming successful communication.
- The switch forwards the frames to the correct destination.

These steps illustrate how even a simple connectivity test involves several underlying processes.

---

## Screenshots

### Network Topology
![Network Topology](images/01_network_topology.png)

### Packet Simulation
![Packet Simulation](images/02_packet_simulation_icmp.png)

### Ping Output
![Ping Output](images/03_ping_output.png)

---

## Reflection

This experiment was part of my effort to combine theoretical learning with hands-on observation.

Seeing these processes occur step by step made the concepts much clearer than simply reading about them. It reinforced the importance of experimenting and documenting what I learn as I continue developing my technical skills.

This lab represents an early step in my broader journey of exploring how technology works beneath the surface.
