**### HANDS-ON PRACTICAL NETWORK FORENSIC ANALYSIS PROJECT USING NETWORK MINNERS**

Networkminner is an  important open source forensic analysis tools. it can be used for passive sniffer that  fingerprint host, session, open port without sending nay traffic over the network. It can also serve as a PCAP that reassemble files and certificate from capture traffic  for analysis.
Networkminner is a n important tools used for  traffic sniffing, parsing PCAP files,protocol analysis, OS fingerprinting( identifying te OS in use), file extration, credential  grabbing etc. 
There are three type of data to be capture:
- Live traffic
- log file
- Traffic capture
There are 2 diffenret mode of NetworkMinner:
1: Sniffer mode : This is use for  packetsniffing even if the primry usag is network forensic analysis.
2.Packet snarfing/processing mode:This operation mode is mainly suggested to grab the "low hanging fruit" before diving into a deeper investigation.

With the information aquired i wil be doin the project belwo using TRYHACKME exercise file:

**TASK 1 :Use the "~/Desktop/Exercise Files/mx-3.pcap" file to answer the questions below.
What is the total number of frames?**
In the project abocve, i uploaded the file mx-3 cap and look for the total number of frames which  was **460 frames**
<img width="482" height="350" alt="Image" src="https://github.com/user-attachments/assets/7dc50b5e-6a20-4a9d-99d4-aa52535d76ae" />

**TASK 2: How many IP addresses use the same MAC address with host 145.253.2.203?**

In this task, i select the ip address from the host dropdown, click on the host ip address, and display the  mac addrss on the same host MAC address s shown in the screenshot below:

<img width="400" height="242" alt="Image" src="https://github.com/user-attachments/assets/2ee054a1-cd7f-4230-9808-b538489fbaf6" />

**TASK 3: How many packets were sent from host 65.208.228.223?**
In this task, by clicking on the ip address i was able to seee how many packet was sent from the host, which ws 72 packet.

<img width="365" height="256" alt="Image" src="https://github.com/user-attachments/assets/243cd6ac-18f8-425c-888c-c9cabcb22ee9" />

**TASK 4: What is the name of the webserver banner under host 65.208.228.223?**
I clicked in the ip_address an open the host pan tohace a look at the banner which is **"APACHE"**

<img width="356" height="240" alt="Image" src="https://github.com/user-attachments/assets/6151c5f8-04db-473f-a2af-a19498c21571" />

**TASK 5: Use the "~/Desktop/Exercise Files/mx-4.pcap" file to answer the questions below.
What is the extracted username for the 02694W-WIN10 host?**
In the task , i make use of Networkmiver version 2.7.2 from the  packet credential section i was able to find the username to be :#**B\Administrator**

<img width="374" height="104" alt="Image" src="https://github.com/user-attachments/assets/3abf754b-0f13-467a-af31-f0a8c01d2eae" />

**TASK 6: What is the extracted password for the user logged into the 02694W-WIN10 host?
Enter the full NTLM hash.**
 In the credential  section we  can find the password of the user:

<img width="391" height="155" alt="Image" src="https://github.com/user-attachments/assets/2c011f01-45dc-47ba-91e6-4498cd49daf7" />

TASK 7: Use "~/Desktop/Exercise files/mx-7 pcap" file to answer the questions below
What is the name of the Linux distro mentioned in the file associated with frame 63602?
(Note: If there are no results associated with this frame, check out frame 63075)

In this task i search for 63602 and i founc no result, then i filter for frame 63075  which display the name  of the  name of the Linux distro as shown in the screenshot below:

<img width="471" height="164" alt="Image" src="https://github.com/user-attachments/assets/413fef27-9289-4abc-9583-14f9f0aef117" />

<img width="335" height="232" alt="Image" src="https://github.com/user-attachments/assets/f3257738-8333-4e33-9a6c-8481b182cdc7" />

TASK 8: What name and surname are mentioned in the file associated with frame 76469?
(Note: If there are no results associated with this frame, check out frame 75942)

In this task, i search for the farem 75942 and view the frame to reveal the name and surname of the frame  as shown in the screenshot below
<img width="449" height="197" alt="Image" src="https://github.com/user-attachments/assets/9b353755-06b7-49ef-b28c-ef31621b9fc9" />

TASK 9:What is the source address of the image "ads.bmp.2E5F0FD9[1].bmp"?
I clicked on the images which display the all picture to select from and this reval the soirce ip_address as shwon in the picture below:

<img width="460" height="343" alt="Image" src="https://github.com/user-attachments/assets/c769d839-f00a-4956-8b4e-c208ef915e46" />

TASK 10: What is the frame number of the possible TLS anomaly?

<img width="417" height="273" alt="Image" src="https://github.com/user-attachments/assets/9be7191d-777e-4d47-a829-03286ab66aa3" />

TASK 11:" Use "~/Desktop/Exercise files/mx-9" file to answer the questions below
Which platform sent an email with the subject starting with "You have more..."?
In this task, i make use of the message  sections, and search for the platform the stated subject as shown below to be from facebook as shown below 

<img width="494" height="404" alt="Image" src="https://github.com/user-attachments/assets/7a02dcbc-a751-42d2-b240-8e1918c1dfc7" />

TASK 12: What is the email address of Branson Matheson?

<img width="307" height="112" alt="Image" src="https://github.com/user-attachments/assets/e8689844-c925-4636-8bb1-20184bf8a4fc" />
As shown above the email associated with Branson Matheson is _branson@sandsite.org_

TASK 13:Use the ~/Desktop/Exercise Files/case1.pcap file to answer the questions below.
What is the full OS name of the host 131.151.37.122?
In this task we have to open tge frame and seach for the operating system of the said ip address as shown innthe screenshot below: 
**_Windows - Windows NT 4_** 

<img width="388" height="320" alt="Image" src="https://github.com/user-attachments/assets/2fe5cf3d-a0e1-474e-a62a-3f473294d7b2" />

TAK 14: Investigate the hobetween 131.151.37.122 and 131.151.32.91.
How many bytes were sent by the client (*.32.91) through port 1065?

This task ask or the number opf bye sent between the ip 131.151.37.122 and 131.151.32.91 on port 1065,by opeining the pane of both ip adrres i was able to fimd out the  number of packet  to be **_192_**

<img width="389" height="248" alt="Image" src="https://github.com/user-attachments/assets/3521e661-d259-41a9-b5f2-18106a1c5b79" />

TASK 15: Investigate the communication between 131.151.37.122 and 131.151.32.21.
How many bytes were sent back by the server (*.37.122) through port 143?

I opened the ip_address pane  to revael the total byte stn back by the server to be 20769
as reveal in the screenshopt below:

<img width="374" height="328" alt="Image" src="https://github.com/user-attachments/assets/c73591ae-3c2e-4220-a6ec-8d950f86ebc6" />

TASK 16 :What is the sequence number of frame number 9? 
In this task i make use of version 1.6.1 to check on frame 9 and the sequence number as shown in the screenshot below the sequence number is _2AD77400_

<img width="384" height="251" alt="Image" src="https://github.com/user-attachments/assets/7f551a35-340c-40cc-87ce-edc3dc575ace" />

TASK 17: What is the number of the detected "content types"?
In this task i use the veersion 2.7 to filter from the parameter and detected 2 content type  _(plain/text and the multipart/mixed)_
as shown below

<img width="425" height="274" alt="Image" src="https://github.com/user-attachments/assets/7107d3a9-363d-4c2f-863b-e11bec0c617f" />

TASK 18: Use the ~/Desktop/Exercise Files/case2.pcap file to answer the questions below.
What is the USB product's brand name?
I  upload the file case.2, click on file and type usb on the filter keyword space then look for the usb name which was found as Asix as shown innthebscreenshot below:

<img width="1100" height="205" alt="Image" src="https://github.com/user-attachments/assets/ed5a06da-8eaa-45c3-90a9-0f3b8e16b2af" />

TASK 19: What is the name of the phone model?
I found the phine model by clicking on image scroll; down to the picture with a phone brand name .
As shown in the screenshot below:

<img width="401" height="239" alt="Image" src="https://github.com/user-attachments/assets/dbdb9e18-02c5-4776-8787-8336a7bf3ff9" />

TASK 20 : What is the source IP of the fish image? 
In this case i went to file and type fish in the filter keyword to get  the source ip is shown below:

<img width="404" height="265" alt="Image" src="https://github.com/user-attachments/assets/8e0db2d3-1977-473e-b51e-037ef9cb298f" />
TASK 21: What is the password of the homer.pwned.se@gmx.com?

In this task, i went to  credential and scroll down to homer.pwned.se@gmx.com is locate to fine the password to be _spring2015_

<img width="409" height="365" alt="Image" src="https://github.com/user-attachments/assets/7fa87ddb-8dd4-4d32-9e6e-58456dbcadb5" />

TASK 22: What is the DNS query of frame 62001?

In the task i click on DNS, i filter 62001 and scroll to the dns query which is  _pop.gmx.com_
As shown below:

<img width="409" height="276" alt="Image" src="https://github.com/user-attachments/assets/ea93bcdc-654f-4820-8a7d-f5e439ae2b47" />

