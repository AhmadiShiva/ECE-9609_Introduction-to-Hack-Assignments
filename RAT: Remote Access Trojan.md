![01_What_Is_RAT](https://user-images.githubusercontent.com/90869009/158062109-365517b6-ab1f-4191-90e2-dbadea787e44.jpg)
**RAT** stands for **Remote Access Trojan** or **Remote Administration Tool**. This type of tool is one of the most terrible security threats for both individuals and organizations. Using RAT, a hacker can take complete control of victim’s computer and do anything with it.

## *What Can a RAT Do?*
RAT is often used by **APT attackers** to gain interactive access to a victim's computer and steal confidential data. Once RAT is installed on the victim's computer system, the hacker can do almost anything with the system. 

Some of these malicious activities are as follows:
  * Monitoring victim's screen.
  * Start and open remote applications such as webcam, music player, etc.
  * Infect system files.
  * Install keyloggers to capture keys entered by the victim.
  * Use system as a zombie system for DDOS attacks.
  

## *Can RATs Be Useful?*
Although most RATs are malicious, there are some useful RATs. Programs like **TeamViewer** are valuable RATs used to remotely control systems over the Internet and to transfer files and support systems. When there is a technical problem with any of the computers at workplaces, the corporate IT guys may use a RAT to gain access to the computer and resolve the issue.

## *RAT Attack Procedure*
"RAT is a malware program that includes **a back door for administrative control** over the target computer"[[1]](https://www.techtarget.com/searchsecurity/definition/RAT-remote-access-Trojan). A backdoor is a way to get access to a computer system or encrypted data by circumventing the system's normal security measures. Email attachments, USB memory, and file bundles are all common ways for RAT to get into a system. RATs are typically delivered as an email attachment or downloaded **invisibly** with a user-requested program, such as a game or any other popular application. Once the host system has been infiltrated, the intruder can use it to spread RATs to other computers that are vulnerable, forming a botnet[[1]](https://www.techtarget.com/searchsecurity/definition/RAT-remote-access-Trojan). 

RATs are often built on the **Client/Server architecture**. The attacker has control over the client, and the server is installed on the victim's PC. To implement remote control for the victim host, the attacker utilizes the client to control the server[[2]](https://www.mdpi.com/2079-9292/9/11/1894/htm).
![02_The_Whole_Communication_of_RAT](https://user-images.githubusercontent.com/90869009/158065913-0f63b41c-fea8-4c16-ba2e-9dc57527e3c0.jpg)

## *Two Well-known and Highly Prolific Platforms for Windows RAT*
In the following, we will consider building a Windows RAT through two popular frameworks :
 1. njRAT
 2. Metasploit

### *njRAT*
This Remote Access Trojan (RAT) is a simple.NET backdoor that is popular among amateurs, especially in the Middle East. The majority of users are low-level criminals, and it is frequently delivered via drive-by downloads or phishing attacks. njRATs files frequently include custom packets (.PDF) to avoid detection by traditional antivirus solutions, and once installed, the malware is capable of hijacking infected systems[[3]](https://www.zdnet.com/article/njrat-secures-top-spot-as-most-active-malware-on-networks-in-2017/).

Here is an example of accessing and hacking a system with Windows OS via the njRAT tool(njRAT-v0.8d):
![nj_RAT_01](https://user-images.githubusercontent.com/90869009/158079991-4731a887-2408-4adf-b9eb-93ee868146b9.jpg)
By clicking on the njRAT.exe file, the user(hacker) accesses the application's environment. After entering the desired port, creating the malicious file will start by clicking the Build button.
![nj_RAT_02](https://user-images.githubusercontent.com/90869009/158080171-0ea05f48-9b76-47e7-b3c5-a0ef9e53cb26.jpg)
In Builder Windows, the local IP of the hacker's system will enter in the Host section. Of course, an IP provided by a  VPS or Port Forwarding approach would be more effective.
![nj_RAT_03](https://user-images.githubusercontent.com/90869009/158080884-ba144552-6756-487d-82e2-5486390f6667.jpg)
A nickname could be set for the file (Vic Time Name Section). From Dictionary Drop-Down List, the directory of the RAT file in the target (victim's) system could be specified. A name should be set for the exe file, and finally,  the RAT file will be created by clicking on the Build button.
![nj_RAT_04](https://user-images.githubusercontent.com/90869009/158081537-aa19aadd-37dc-4b0f-aef7-0655bdeaee74.jpg)
In case of running exe file on the victim's system, through any of the methods mentioned earlier, the hacker will be able to access full control of the target system.
![nj_RAT_05](https://user-images.githubusercontent.com/90869009/158082028-615a4771-4e18-4733-9d15-f307c519b463.jpg)
The hacker could access the folders and files of the victim system just by Right-Click on the record of the victim: Manager --> File Manager
![nj_RAT_06](https://user-images.githubusercontent.com/90869009/158082154-d97c5cce-f11c-410d-b472-fca85d5fb4a4.jpg)

Similarly, the hacker can perform the following activities:
  * Process Managing ( RC --> Manager --> Process Manage)
  * Running CMD Commands in PowerShell ( RC --> Manager --> Remote Shell)
  * Recording and listening to the microphone ( RC -->  Manager --> Microphone)
  * Viewing and downloading saved passwords in browser ( RC --> Manager --> Get Passwords)
  * Remote Desktop ( RC --> Remote Desktop)
  * Install keyloggers to capture keys entered by the victim ( RC --> Keylogger)
  *etc.
  
![nj_RAT_07](https://user-images.githubusercontent.com/90869009/158083622-ece89da7-731b-449e-846f-ada73c293196.jpg)
Finally, access to the victim system can be terminated by the hacker(RC --> Keylogger --> Close).











### *Metasploit*
Metasploit is one of the most popular penetration test frameworks that make the penetration test process easier for professionals. In addition to penetration test experts, Metasploit is famous among hackers. This framework speeds up the hacking operation and makes it more accessible.










