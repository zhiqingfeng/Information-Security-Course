# H4 Hash

## Read the summarize

### Schneier 2015: Applied Cryptography

- 2.3 **ONE-WAY FUNCTIONS**
  
  A one-way functions is a mathematical operation that is easy to compute in one direction, but it's difficult to reverse. By using on one-way functions, the users can securely exchange data without needing to worry about the data being intercepted or tampered with. The sender and the receiver could transfer the data by usint the same function. This ensure the data is secure and not able to attack. (One-way means that it is not possible to reverse the output back into the original input)
  
- 2.4 **ONE-WAY HASH FUNCTIONS**

  The one-way hash functions it's central to modern cryptography. One-way hash functions are another building block for many protocols. The message authentication codes is a very good example from the material. MAC also called data authentication code (DAC) which is a one-way has function with the addition of a secret key. Only the person who with the key can verify the hash value. (Used the data such as passwords).
  For example SHA-2(Secure Hash Algorithm 2). This is uses from 64 to 80 rounds of cryptography operations and it is common to validate and sign digital security certificates and documents.
  
  
## Install Hashcat.

Already installed Hashcat during the class. 
```
sudo apt-get install hashcat
```

## Crack this hash: 8eb8e307a6d649bc7fb51443a06a216f

1. Intsall Hashcat

Faced this issue.

<img width="736" alt="image" src="https://user-images.githubusercontent.com/95883827/218669291-3cf19a5a-3c16-4f57-8130-f365d9be19fd.png">

*Trying to find the solution, will update later. 
*I have tried many ways to configurated the network seting, but it do not allow me access github.com and terokarvinen.com

## Compile John the Ripper, Jumbo version.

1. Up-to-date
  ```
   sudo apt-get update
  ```
2. Prerequisties
  ```
   sudo apt-get -y install micro bash-completion git build-essential libssl-dev zlib1g zlib1g-dev zlib-gst libbz2-1.0 libbz2-dev atool zip wget
  ```
3. Clone the git 
  ```
   git clone --depth=1 https://github.com/openwall/john.git
  ```
4. Run the configure 
   
   In this step, I am not able to run the configure, then i install it.
   
   <img width="860" alt="image" src="https://user-images.githubusercontent.com/95883827/218572502-2fd0b242-7ea9-491d-af81-c034a401fc3f.png">

  ```
   /john/src/./configure
  ```
  
  ![image](https://user-images.githubusercontent.com/95883827/218572679-0310be35-12b7-43dd-802f-488931ab5a0c.png)

5. Compliation 
  In this step, make is not working.
  
  ![image](https://user-images.githubusercontent.com/95883827/218572900-157e7634-5256-4be0-9f40-62d139c48db8.png)

*Trying to find the solution, will update later. 
*Do not find the solution for it.


## Crack a zip file password
*This section is not working because i can't find out the how to run make command.
