# Wireshark Investigation: Deciphering IcedID Malware Communications

## Introduction
Welcome! Today, I dive into a detailed examination of malware intricacies using Wireshark’s insightful capabilities. My focus will be on analyzing the “Cold as Ice: IcedID” traffic analysis scenario presented by https://malware-traffic-analysis.net

For those keen on a hands-on experience using their own setup, you’re encouraged to download the PCAP file designated for the “Cold as Ice: IcedID” case. This exercise is just one of the many authentic simulations available at malware-traffic-analysis.net. Access and download the necessary files for this specific investigation through the link provided (https://unit42.paloaltonetworks.com/wireshark-quiz-icedid/)

## Critical Alert: Safely Analyze Malicious Network Traffic in a Secure Environment
Understanding the risks associated with PCAP files filled with malicious content is crucial, as these files may contain payloads that pose a threat to your system’s security. Simply opening a file without the appropriate safeguards could inadvertently trigger an infection on the device being used for analysis.

When it comes to network analysis, particularly the examination of PCAP files that may contain dangerous data, maintaining a high level of operational security is paramount. Although Wireshark is a powerful instrument for conducting such analysis, it’s important to bear in mind that it does not offer automatic protection against the hidden threats within the data you’re investigating.

## The Scenario: Cold as Ice (IcedID)

In this section, I focused on the IcedID scenario, a compelling and intricate case. IcedID is a type of malware recognized for its proficiency in stealing information, encompassing the acquisition of sensitive data such as passwords, browser history, and cryptocurrency details from compromised systems. It frequently disseminates through deceptive tactics like phishing emails or tainted software downloads. Our goal in this analysis is to examine network traffic related to this malware to discern its actions and pinpoint possible routes of infection.

In my investigation of the IcedID scenario using Wireshark, we are equipped with crucial details that will greatly enhance my analysis.

### Local Area Network (LAN) Details:
   - LAN segment range: 10.4.19[.]0/24 (10.4.19[.]1 through 10.4.19[.]255)
   - Domain: boogienights[.]live
   - Domain controller IP address: 10.4.19[.]19
   - Domain controller hostname: WIN-GP4JHCK2JMV
   - LAN segment gateway: 10.4.19[.]1
   - LAN segment broadcast address: 10.4.19[.]255

### During the course of my analysis, I will address the questions listed on the scenario’s webpage:
   - What is the date and time in UTC the infection started?
   - What is the IP address of the infected Windows client?
   - What is the MAC address of the infected Windows client?
   - What is the hostname of the infected Windows client?
   - What is the user account name from the infected Windows host?
   - Is there any follow-up activity from other malware?



