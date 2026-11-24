# Network Forensics CTF

An office workstation made a series of unusual network requests. Your only evidence is a [packet capture](./evidence/incident.pcap) from the fictional company network.

## Your investigation

Open `incident.pcap` in Wireshark. Identify the workstation that made the unusual requests and trace its activity. Which file did it retrieve? What clues in the traffic let you open that file and recover the flag?

## What to submit

- The workstation’s IP address and the name of the file it retrieved.
- The flag exactly as it appears in the recovered file.
- A brief explanation citing the packet numbers that identify the workstation, show the file transfer, and reveal the clues you used.