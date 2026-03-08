# Deep Packet Inspection (DPI) Engine

A C++ based **Deep Packet Inspection (DPI) engine** that analyzes network traffic from PCAP files, classifies applications using TLS SNI extraction, and applies rule-based filtering for IPs, domains, and applications.

## Features

* Parse **Ethernet, IP, TCP, and UDP headers** from PCAP files
* Track network connections using the **Five-Tuple model**
* Extract **TLS SNI and HTTP Host** to identify applications
* Classify traffic such as **YouTube, Facebook, Google, etc.**
* **Rule-based blocking** for IP addresses, domains, and apps
* **Multi-threaded packet processing** for faster traffic analysis
* Generate **traffic statistics and application reports**

## Tech Stack

C++, Multithreading, TCP/IP Networking, TLS/SNI Analysis, PCAP Processing, Deep Packet Inspection, CMake, Git


## Build

```bash
mkdir build
cd build
cmake ..
make
```

## Run

```bash
./packet_analyzer input.pcap output.pcap
```

Example with blocking rules:

```bash
./packet_analyzer input.pcap output.pcap --block-app YouTube --block-domain facebook
```

## How It Works

1. Reads packets from a **PCAP capture file**
2. Parses network protocol headers
3. Extracts **SNI from TLS Client Hello**
4. Classifies application traffic
5. Applies filtering rules and generates statistics

## Use Cases

* Network traffic analysis
* Security monitoring
* Application usage detection
* Network policy enforcement

you want, I can also give you a **slightly better GitHub README (with diagrams and badges)** that will make your repo **look much more professional to recruiters.**
