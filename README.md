
Enumeration Techniques

# Explore Google hacking and enumeration 
## Name: Yathin Reddy T
## Reg num: 212223100062
# AIM:

To use Google for gathering information and perform enumeration of targets

## STEPS:

### Step 1:

Install kali linux either in partition or virtual box or in live mode

### Step 2:

Investigate on the various Google hacking keywords and enumeration tools as follows:


### Step 3:
Open terminal and try execute some kali linux commands

## Pen Test Tools Categories:  

Following Categories of pen test tools are identified:
Information Gathering.

Google Hacking:

Google hacking, also known as Google dorking, is a technique that involves using advanced operators to perform targeted searches on Google. These operators can be used to search for specific types of information, such as sensitive data that may have been inadvertently exposed on the web. Here are some advanced operators that can be used for Google hacking:

site: This operator allows you to search for pages that are within a specific website or domain. For example, "site:example.com" would search for pages that are on the example.com domain.
Following searches for all the sites that is in the domain yahoo.com
![image](https://github.com/user-attachments/assets/7814b78d-49a6-4345-92eb-2b7325f9c1dc)


filetype: This operator allows you to search for files of a specific type. For example, "filetype:pdf" would search for all PDF files.
Following searches for pdf file in the domain yahoo.com
![image](https://github.com/user-attachments/assets/a276231b-4320-4214-a4fa-5ddd928854fa)




intext: This operator allows you to search for pages that contain specific text within the body of the page. For example, "intext:password" would search for pages that contain the word "password" within the body of the page.
![image](https://github.com/user-attachments/assets/5281302f-0ec0-4f36-a570-e0234ee314f1)


inurl: This operator allows you to search for pages that contain specific text within the URL. For example, "inurl:admin" would search for pages that contain the word "admin" within the URL.
![image](https://github.com/user-attachments/assets/c0f6dce4-56d3-4361-b334-478ee82349c1)


intitle: This operator allows you to search for pages that contain specific text within the title tag. For example, "intitle:index of" would search for pages that contain "index of" within the title tag.
![image](https://github.com/user-attachments/assets/578e220d-b3bf-4a6a-8d19-bbf8be2541b9)


link: This operator allows you to search for pages that link to a specific URL. For example, "link:example.com" would search for pages that link to the example.com domain.
![image](https://github.com/user-attachments/assets/4dae0484-e009-44f1-8200-f519d277a249)


cache: This operator allows you to view the cached version of a page. For example, "cache:example.com" would show the cached version of the example.com website.
![image](https://github.com/user-attachments/assets/36a61382-8611-4b1f-9bf0-a1b433f02aaa)

 
#DNS Enumeration


##DNS Recon
provides the ability to perform:
Check all NS records for zone transfers
Enumerate general DNS records for a given domain (MX, SOA, NS, A, AAAA, SPF , TXT)
Perform common SRV Record Enumeration
Top level domain expansion
## OUTPUT:
![image](https://github.com/user-attachments/assets/3ad7e1d5-a40d-49cb-b4f1-f67a36212bcd)
![image](https://github.com/user-attachments/assets/e3a58724-651a-4beb-a254-a740546d71ac)









##dnsenum
Dnsenum is a multithreaded perl script to enumerate DNS information of a domain and to discover non-contiguous ip blocks. The main purpose of Dnsenum is to gather as much information as possible about a domain. The program currently performs the following operations:

Get the host’s addresses (A record).
Get the namservers (threaded).
Get the MX record (threaded).
Perform axfr queries on nameservers and get BIND versions(threaded).
Get extra names and subdomains via google scraping (google query = “allinurl: -www site:domain”).
Brute force subdomains from file, can also perform recursion on subdomain that have NS records (all threaded).
Calculate C class domain network ranges and perform whois queries on them (threaded).
Perform reverse lookups on netranges (C class or/and whois netranges) (threaded).
Write to domain_ips.txt file ip-blocks.
This program is useful for pentesters, ethical hackers and forensics experts. It also can be used for security tests.
![image](https://github.com/user-attachments/assets/0feedc0f-8323-4bbf-80bf-a14840278191)


##smtp-user-enum
Username guessing tool primarily for use against the default Solaris SMTP service. Can use either EXPN, VRFY or RCPT TO.
![image](https://github.com/user-attachments/assets/38dedc49-4a20-42b5-b1a9-1ca7572c687d)


In metasploit list all the usernames using head /etc/passwd or cat /etc/passwd:
![image](https://github.com/user-attachments/assets/5a825064-6565-480f-b305-0fe3b7df8849)



select any username in the first column of the above file and check the same
![Screenshot 2025-04-21 112437](https://github.com/user-attachments/assets/bb619a68-23cd-4e0c-bbef-47fdfc360171)


#Telnet for smtp enumeration
Telnet allows to connect to remote host based on the port no. For smtp port no is 25
telnet <host address> 25 to connect
and issue appropriate commands

 ![image](https://github.com/user-attachments/assets/2a6ed999-b5c4-4f33-8974-db2f7740dc75)

 ##Output
  
  

## nmap –script smtp-enum-users.nse <hostname>

The smtp-enum-users.nse script attempts to enumerate the users on a SMTP server by issuing the VRFY, EXPN or RCPT TO commands. The goal of this script is to discover all the user accounts in the remote system.


## OUTPUT:

![image](https://github.com/user-attachments/assets/8021c4a3-f338-4f14-92a9-043272b17c02)


## RESULT:
The Google hacking keywords and enumeration tools were identified and executed successfully

