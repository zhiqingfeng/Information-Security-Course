# H3 Attack

## x) Read and summarize 

### Costa-Gazcón 2021: Practical Threat Intelligence and Data-Driven Threat Hunting Chapter 4: Mapping the Adversary (all but "Testing yourself", which is left as voluntary bonus)

- The ATT&CK Framework is a descriptive model used to label and study the activities that a threat actor. The ATT&CK Framework is that it provides a          common taxonomy for the cybersecurity community to describe adversary behaviors.

- **The list of the ATT&CK enterprise's tactics**

  **Reconnaissance**
      Collect as much as information about victim.
              
  **Resource Development**
      This technique tries to cover the process of assessing the resources that the adversary uses.
      
  **Initial Access**
      This is the first step into the victim's environment. Try to get into network by using different entry vectors.
  
  **Execution**
      Running malicious code inside the victim's environment. (esim escalating privileges or exfiltrating information.)
      
  **Persistence**
      The threat actor can stay inside the system for a long time. Even thought the system turn it off or on.
      
  **Privilege Escalation**
      The threat actors get inside the enterprise network through an unprivileged account.
      
  **Defense Evasion**
      Avoiding being detected by the victim's defenses which could installing or uninstalling the software to remove their track.
      
  **Credential Access**
      Try to act like they are the illega user to access the system.
      
  **Discovery**
      Group all the activities that the threat actor did so that know about the vitcim's environment.
      
  **Lateral Movement**
      The threat actor can try to transfer from one system to another until they reach their target.
      
  **Collection**
      Gathering information from the victim's environment so that they can leak it later.
      
  **Command and Control**
      The threat actor communicating with the systems under its control.
  
  **Exfiltration**
      Try to remain undetected while the threat actior stealing information.
      
  **Impact**
      All attempts to prevent the victim from accessing his/her system, including manipulating or destroying it, 
       


- **The ATT&CK Matrix**
  
  <img width="1726" alt="image" src="https://user-images.githubusercontent.com/95883827/217062531-3dc59341-7624-48f4-85f9-0f60a2bbb71c.png">
  
  *All the technique pages follow the same pattern: the technique's name, a list of sub-techniques, a description of the technique, the scorecard that the platforms operate on, and the main data sources for finding that type of activity*

     - One of the best tools for working with the ATT&CK Matrix in an interactive way: **the ATT&CK Navigator**.
     
     - *The ATT&CK Navigator is a web-based tool for annotating and exploring ATT&CK matrices. It can be used to visualize defensive coverage, red/blue     team planning, the frequency of detected techniques, and more.*
     
     - <img width="843" alt="image" src="https://user-images.githubusercontent.com/95883827/217063595-b36a9697-8104-4477-97d3-71bb49eb7027.png">
     
- **Mapping with ATT&CK**
   Formbook is an infostealer that has been around since at least 2016 and has been advertised in hacking forums by the user ng-Coder.
   
   - Steal authorization and login credentials: Credential Access:
     a) T1555 – Credentials from Password Stores

     i) T1555.003 – Credentials from Web Browsers

     b) T1056 – Input Capture

     i) T1056.001 – Keylogging

   - Keylog information, even if victims use a virtual keyboard, auto-fill, or if they copy and paste: Collection:
     a) T1056 – Input Capture

     i) T1056.001 – Keylogging

   - Take screenshots: Collection:
     
     a) T1113 – Screen Capture
 
 
 ## y) Write an answer with references (this subtask does not require tests with a computer). Answer in the context of Mitre Att&ck, and pick examples that       are different from the chapter in task x.

 ### Define tactic and give an example.
 
 - In this section, I am defining the teactic called 'Collection'. This is gathering information from the victim's environment so that they can leak it later. This tactic is included 17 techniques.
 - Defination link: [Collection](https://attack.mitre.org/tactics/TA0009/).
 - Example: Could be collect information by browsers, audio, video, and email. Common collection methods include capturing screenshots and keyboard input.
 
 ### Define technique and subtechnique, and give an example of each.
 
 - Please see the screenshot of each tecniques and its subtechnique.
  <img width="373" alt="image" src="https://user-images.githubusercontent.com/95883827/217070212-9fb1bf9a-dd80-4fd8-ba8a-021eb54613c4.png">
  <img width="359" alt="image" src="https://user-images.githubusercontent.com/95883827/217070610-e7f14124-b200-4d68-8ca2-c111d11b1068.png">


 ### Define procedure, and give an example of each.
 
 *I am defining procedure of each tecnique here.*
 
 1. **Adversary-in-the-Middle**
    <img width="1103" alt="image" src="https://user-images.githubusercontent.com/95883827/217073019-a3a26b2e-07f6-4600-9dba-9d040ea5abb6.png">

 2. **Archive Collected Data**
    <img width="956" alt="image" src="https://user-images.githubusercontent.com/95883827/217073606-d26d6b57-b659-4fa6-ac57-5bdfff159432.png">

 3. **Audio Capture** (bandook)
    <img width="1021" alt="image" src="https://user-images.githubusercontent.com/95883827/217073670-ff610afe-9123-483f-825a-91d920bdb488.png">
 
 4. **Automated Collection** (AppleSeed)
    <img width="1085" alt="image" src="https://user-images.githubusercontent.com/95883827/217073867-94c32cd3-439e-488c-81ad-ca061f880fd0.png">

 5. **Browser Session Hijacking**
    <img width="1182" alt="image" src="https://user-images.githubusercontent.com/95883827/217073978-cd2075c3-d646-4827-aa1d-c861b816f280.png">
    
 6. **Clipboard Data**
    
    <img width="810" alt="image" src="https://user-images.githubusercontent.com/95883827/217075505-16f8a406-ad85-4c57-ae88-9886038b53bc.png">

 7. **Data from Cloud Storage**
    <img width="1244" alt="image" src="https://user-images.githubusercontent.com/95883827/217074148-f117bfaa-4e4f-4ff2-8413-58ebb2fc3d14.png">

 8. **Data from Configuration Repository**
    
 9. **Data from Information Repositories**
 
 10. **Data from Local System** (AppleSeed)
    <img width="1037" alt="image" src="https://user-images.githubusercontent.com/95883827/217074365-cdbcd1bb-7b00-47d4-9161-0a0517c3bc0a.png">

 11. **Data from Network Shared Drive**
    <img width="1245" alt="image" src="https://user-images.githubusercontent.com/95883827/217074529-ea631d5b-dae6-45a9-9a31-7ca0ed2b6eec.png">

 12. **Data from Removable Media** (AppleSeed)
    <img width="854" alt="image" src="https://user-images.githubusercontent.com/95883827/217074649-632528cf-375f-47e8-b329-9e4597238c82.png">

 13. **Data Staged**
    <img width="1246" alt="image" src="https://user-images.githubusercontent.com/95883827/217074752-6c4eeaf9-0ac4-4eb7-a773-0f5d9d303f33.png">

 14. **Email Collection** (This is very commond)
    <img width="948" alt="image" src="https://user-images.githubusercontent.com/95883827/217074825-f7e6284f-fc78-41fd-9c83-ecaa46687571.png">

 15. **Input Capture** 
  *During normal system usage, users often provide credentials to various different locations, such as login pages/portals or system dialog boxes. *
    <img width="1235" alt="image" src="https://user-images.githubusercontent.com/95883827/217074905-e450967c-7e66-4693-a4d5-91b484a32537.png">

 16. **Screen Capture**(AppleSeed)
    <img width="947" alt="image" src="https://user-images.githubusercontent.com/95883827/217075077-b531042b-8e47-43b8-ac22-79d5fdb5e501.png">

 17. **Video Capture**(Bandook)
    <img width="898" alt="image" src="https://user-images.githubusercontent.com/95883827/217075165-61209b54-e9db-4c41-8511-dc072886b791.png">


## Webgoat: A3 Sensitive data exposure

### Insecure Login: 2 Let's try

*Encryption is a tool for secure communication. In this section, I will be understand of packet sniffer usage and able to intercept and read an unencrpted requests.*

- Using this vidoe to understood the point of this task [OWASP WebGoat Sensitive Data Expo Insecure Login](https://www.youtube.com/watch?app=desktop&v=qawrnAIPDRs&ab_channel=TudellTechTV)

Now try to get the username and password on WebGoat.

1. Run the WebGoat from terminal and then log in.
   <img width="513" alt="image" src="https://user-images.githubusercontent.com/95883827/217078347-c696da8f-8ebe-4e6c-8880-ec72b59c1f72.png">

2. Opened 'inspect'to located the username and password.
   <img width="593" alt="image" src="https://user-images.githubusercontent.com/95883827/217078509-43b50efe-e31c-4670-982d-59d34fc01546.png">

3. Go to 'Network' and press 'Log in'.
4. I saw the there has a wrong code called 405, press it and go to 'Request'
   <img width="757" alt="image" src="https://user-images.githubusercontent.com/95883827/217078910-85539f4f-4fec-43ed-bc1d-da18caee7ba3.png">
   <img width="558" alt="image" src="https://user-images.githubusercontent.com/95883827/217078965-886b1234-148c-4de5-be71-ca4a4d0fe5ca.png">

5. Input the username and password I find from the 'Request'
   <img width="1105" alt="image" src="https://user-images.githubusercontent.com/95883827/217079101-b1b0729b-9ee7-4a8e-ba44-7537c3f58ec0.png">
6. Worked and login successfully. :) 

## n) Voluntary bonus: "Testing yourself" in Costa-Gazcón: Practical Threat Intelligence and Data-Driven Threat Hunting Chapter 4: Mapping the Adversary
*I might be do it a bit later! :) 

## Sources

**Tasks**

[Tero-Karvinen_h3 Attaaack](https://terokarvinen.com/2023/information-security-2023/)

**Lectures**
[Chapter 4: Mapping the Adversary](https://learning.oreilly.com/library/view/practical-threat-intelligence/9781838556372/B13376_04_Final_SK_ePub.xhtml#_idParaDest-70)

[MITRE ATT&CK® ](https://attack.mitre.org/)

**External**
[OWASP WebGoat Sensitive Data Expo Insecure Login](https://www.youtube.com/watch?app=desktop&v=qawrnAIPDRs&ab_channel=TudellTechTV)
