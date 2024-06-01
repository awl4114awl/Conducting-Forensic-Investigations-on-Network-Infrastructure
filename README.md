<p align="left">
<img src="https://i.imgur.com/t23TXuR.png" height="20%" width="20%" alt="daubert standard"/>
</p>

Introduction

Network forensics refers to the investigation of network traffic patterns and data captured in transit between computing devices. Network forensic techniques can provide insight into the source and scope of an attack, as well as supplement investigations of information left behind by intruders. By investigating the causes of a breach, and using that knowledge to build stronger security controls, organizations can work to prevent or mitigate future breaches. With the recent changes in the world, and the massive shift to remote working, the importance of network forensics has increased dramatically, as the rise of breaches, ransomware, and other incidents has grown exponentially.

 

Network forensics has two general purposes. The first consists of monitoring a network for anomalous traffic and identifying intrusions, typically as part of a broader security program. The second consists of analyzing captured network traffic with the objective of reassembling files and parsing communication streams, typically as part of a law enforcement investigation. For both purposes, one of the principal techniques is packet analysis, which involves using a packet capture utility (also called a sniffer) to intercept and record live network traffic, then reviewing the captured packets for evidence. This form of analysis is similar to conducting investigations on drive images and other forms of acquired evidence that have been preserved in a static format. Network forensics is also commonly conducted directly on live networking devices, including routers, switches, and firewalls, due to the fact that shutting down these devices and attempting to image them can potentially result in lost evidence.

 

In this lab, you will learn to capture and analyze network traffic using Wireshark, a popular sniffer and packet analysis utility. You will also learn to access and retrieve evidence directly from both a live router and a live firewall.



Lab Overview

SECTION 1 of this lab has two parts, which should be completed in the order specified.

 

    In the first part of the lab, you will use Wireshark to capture and analyze network traffic.

    In the second part of the lab, you will use basic router commands to gather information about the device itself and the broader network.

SECTION 2 of this lab allows you to apply what you learned in SECTION 1 with less guidance and different deliverables, as well as some expanded tasks and alternative methods. You will take a deeper dive into packet analysis and examine firewall logs.

 

Finally, you will explore the virtual environment on your own in SECTION 3 of this lab to answer a set of questions and challenges that allow you to use the skills you learned in the lab to conduct independent, unguided work - similar to what you will encounter in a real-world situation.



Learning Objectives

Upon completing this lab, you will be able to:

 

    Perform packet capture using Wireshark.

    Perform packet analysis using Wireshark.

    Analyze routers for forensic evidence.

    Examine firewall logs for forensic evidence.

    Identify suspicious network traffic.



Topology

This lab contains the following virtual machines. Please refer to the network topology diagram below.

 

    vWorkstation (Windows: Server 2019)
    router1 (Linux: Ubuntu 16)
    router2 (Linux: Ubuntu 16)
    router3 (Linux: Ubuntu 16)
    pfSense (FreeBSD: pfSense 2.4)
    AttackLinux01 (Linux: Kali)

 

<img src="https://i.imgur.com/s4SNmSn.png" height="40%" width="40%" alt="daubert standard"/>


Tools and Software

The following software and/or utilities are required to complete this lab. Students are encouraged to explore the Internet to learn more about the products and tools used in this lab.

 

    Wireshark
    PuTTY
    Quagga
    pfSense



Deliverables

Upon completion of this lab, you are required to provide the following deliverables to your instructor:

 

SECTION 1

 

    Lab Report file, including screen captures of the following:

 

    Timestamp-sorted traffic
    IP-filtered traffic
    Port-filtered traffic
    TCP push flag-filtered traffic
    Http-filtered traffic
    Router’s version output
    Router’s interface details
    Router's ARP table
    IP routing table
    Currently running configuration

 

    Any additional information as directed by the lab:

 

    None

 

SECTION 2

 

    Lab Report file, including screen captures of the following:

 

    Successful transfer of the secureTopo.png file
    Passive port specified by the FTP server in the Packet Details pane
    Time to live field in the Packet Details pane
    Follow TCP stream window
    Reconstituted PNG file
    Entries in the firewall log
    Resolved entries in the firewall log

 

    Any additional information as directed by the lab:

 

    None

 

SECTION 3

 

    Lab Report file, including screen captures of the following:

 

    Non-RIP route that you discovered on the target router.

 

    Any additional information as directed by the lab:

 

    Record the destination IP address and Port number of the outgoing connection attempt.
