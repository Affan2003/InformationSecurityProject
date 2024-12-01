## IS Project: Exploiting Client-Side Vulnerabilities through User Interaction and Social Engineering


We have defined 5 main tasks(excluding kali setup, lab environment setup and reporting ethical considerations) in our project as follows:


<!-- ### Task 1: Setting Up the Lab Environment4

Create a safe and isolated environment to perform all experiments. Use Virtual Machines (VMs) to ensure no real-world systems are impacted.

Steps to Execute:

* Install Virtual Machine Software: Download and install VM software like VirtualBox or VMware.
* Set Up Kali Linux
* Install a vulnerable OS, such as Windows 7 or a deliberately vulnerable system like Metasploitable or OWASP BWA.
* Configure the VM network to use a Host-Only adapter to ensure no access to the internet but allow communication between VMs.
* Install tools like the Social Engineering Toolkit (SET), Wireshark, and Metasploit on Kali Linux. -->

### Task 1: Hijacking Software Updates and Downloads

Demonstrate how backdoors can be inserted into legitimate software updates or downloads.

Steps to Execute:

* Obtain open-source software for testing purposes.
* Use tools like msfvenom to inject a payload into the installer:
* Use a web server (e.g., Apache) to host the backdoored installer:
* Access the installer via the target VM and execute it.
* Use Metasploit to listen for incoming connections

### Task 2: Backdooring Common Files

Embed malicious payloads into common file formats like PDFs or images.

Steps to Execute:

* Generate a malicious file with msfvenom:
* Use a tool like EvilPDF or manually embed the payload in a PDF.
* Share the backdoored file via email, USB, or hosted on a server.
* Open the file on the target VM and monitor the payload using Metasploit.

### Task 3: Email Spoofing and Social Engineering

Craft phishing emails and gather user information to deceive targets.

Steps to Execute:

* Open the Social Engineering Toolkit:
* Choose “Social Engineering Attacks” and then “Mass Mailer Attack” in SET.
* Customize the phishing email to mimic trusted sources.
* Include a link to the backdoored installer or file.
* Use SET’s built-in email-sending feature or your own SMTP server.
* Monitor if the victim opens the email or downloads the file.

### Task 4: Post-Exploitation Techniques

Demonstrate control of compromised systems through various methods.

Steps to Execute:

* Access the target system via the established Meterpreter session. Use commands like shell for direct access and screenshot to capture the screen.
* Install persistent backdoors using Metasploit’s persistence module.
* Use compromised systems to attack others on the network:

### Task 5: Monitoring and Analysis

Use Wireshark to monitor network traffic for suspicious activities and analyze vulnerabilities.

Steps to Execute:

* Select the network interface connected to the target VM.
* Filter packets by protocols (e.g., HTTP, FTP) to detect and analyze attacks.
* Document observations for later analysis and reporting.

<!-- ### Task 7: Ethical Considerations and Reporting

Ensure the project is conducted ethically and document findings.

Steps to Execute:

* Perform all attacks on virtual machines in an isolated environment.
* Create a report covering vulnerabilities exploited, attack methods, and security recommendations.
* Suggest measures like strong email filters, software update verification, and user awareness training. -->
