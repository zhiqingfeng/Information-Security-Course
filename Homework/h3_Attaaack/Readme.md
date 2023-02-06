# H3 Attack

## x) Read and summarize 

### Costa-Gazcón 2021: Practical Threat Intelligence and Data-Driven Threat Hunting Chapter 4: Mapping the Adversary (all but "Testing yourself", which is left as voluntary bonus)

- **The ATT&CK Framework is a descriptive model used to label and study the activities that a threat actor. The ATT&CK Framework is that it provides a          common taxonomy for the cybersecurity community to describe adversary behaviors.**

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
 
     

