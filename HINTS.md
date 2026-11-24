# Network Forensics CTF: Optional Hints

Open one hint at a time. Each one gives a little more direction.

<details>
<summary>Hint 1: Where do I start?</summary>

Open `incident.pcap` in Wireshark. Enter `http.request` in the display
filter bar and press Enter. Compare the filenames in the Info column.
Which request looks like an ordinary office check, and which one retrieves
something worth investigating? Record the source IP and packet number.

</details>

<details>
<summary>Hint 2: How do I recover the file?</summary>

Go to **File → Export Objects → HTTP**. Find the filename you identified
in the request and save a copy of it.

</details>

<details>
<summary>Hint 3: Where are the password clues?</summary>

Follow the same workstation across two more protocols. Use the `ftp`
filter to inspect its login, then use `dns` to look at the names it
requested. Two of those names contain numbered fragments.

</details>

<details>
<summary>Hint 4: How do the clues fit together?</summary>

Take the hexadecimal characters from the two numbered DNS fragments and
join them in order. Decode the result as text using CyberChef’s **From Hex**
operation. The archive password starts with the FTP password and ends
with the decoded text. Join them without spaces.

</details>