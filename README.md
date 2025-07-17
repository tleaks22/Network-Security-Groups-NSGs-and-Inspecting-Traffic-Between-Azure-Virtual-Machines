# Network-Security-Groups-NSGs-and-Inspecting-Traffic-Between-Azure-Virtual-Machines
In this tutorial, we observe various network traffic to and from Azure Virtual Machines with Wireshark as well as experiment with Network Security Groups.
<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Various Command-Line Tools
- Various Network Protocols (SSH, RDH, DNS, HTTP/S, ICMP)
- Wireshark (Protocol Analyzer)

<h2>Operating Systems Used </h2>

- Windows 10 (21H2)
- Ubuntu Server 20.04

<h2>High-Level Steps</h2>

- Connect to the 2 pre-made VMs "DC-1" and Client1-1 as an admin and then log in as a regular user.
- Create 4 folders with varying access types and permissions. "read, read/write, etc."
- Attempt to view files as the user to see which provides no access.
- Go back to the folder and assign a security group/permissions to it. Then, set a fake user as a member of the group to fully provide access to the user.

<h2>Actions and Observations</h2>

<p>
<img width="628" height="140" alt="image" src="https://github.com/user-attachments/assets/aa2a5d55-4d7f-416b-af70-f57fe7f31080" />

</p>
<p>
Here, I separately signed into 1 VM as an admin and the second as a user.
</p>
<br />

<p>
<img width="512" height="257" alt="image" src="https://github.com/user-attachments/assets/cfba75bb-12bb-428f-8225-520f51d5e01f" />

</p>
<p>
Here, I set up a file with only "read access" to make sure the file couldn't be written on. It could only be read and 
</p>
<br />

<p>
<img width="441" height="178" alt="image" src="https://github.com/user-attachments/assets/9b7548f4-a76b-45cd-8b38-6aedd20b9eee" />

</p>
<p>
Here I attempted to write within a created file that only has "read" access to see if blocked.
</p>
<br />

<p>
<img width="751" height="255" alt="image" src="https://github.com/user-attachments/assets/169da598-95bc-4f64-827e-e5cb3b15d302" />

</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />
