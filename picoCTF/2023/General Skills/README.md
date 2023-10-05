# General Skills

A category where you typically Google your way to get your flag  
  
## Contents
- [money-ware](#money-ware)
- [repetitions](#repetitions)
- [chrono](#chrono)
- Permissions
- useless
- Special

<hr>

## money-ware  
  
### Challenge description
[![image](https://user-images.githubusercontent.com/70287409/228513250-dec6565b-088d-4c0b-be48-0b28a8697502.png)](#Challenge%20description)  
The challenge was to find the name of the Malware and the description gave us some hint about some Bitcoin wallet address `1Mz7153HMuxXTuR2R1t78mGSdzaAtNbBWX`  

### 
[![image](https://user-images.githubusercontent.com/70287409/228514495-db1975d0-510d-43c7-8415-0590e8352924.png)](#)  
The first hint of the challenge suggests that it has something to do with crypto-curreny abuse databases  
  
[![image](https://user-images.githubusercontent.com/70287409/228515230-696ffb04-e551-4e94-8a89-013655c02729.png)](#)  
After some Googling, I found [Bitcoin Abuse](https://www.bitcoinabuse.com/reports/1Mz7153HMuxXTuR2R1t78mGSdzaAtNbBWX) and enetered the wallet address  
  
[![image](https://user-images.githubusercontent.com/70287409/228515771-66e0575f-f81d-4e50-a8a8-1b4aef683b97.png)](#)  
However, the result was reports of Ransomeware which corresponds to this address: not what I was looking for. So I had to Google some more about some ransomware that have something to do with this address  
  
[![image](https://user-images.githubusercontent.com/70287409/228518009-87dd2b30-f51e-4f1d-8859-a9f823d72fe0.png)](#)  
After some digging, I found out that the Ransomeware associated with the address `1Mz7153HMuxXTuR2R1t78mGSdzaAtNbBWX` is known as `Petya`  
[Solved!]  
  
<hr>  
  
## repetitions  
  
### Challenge description  
[![image](https://user-images.githubusercontent.com/70287409/228523307-1fb5e100-e53a-4afe-8755-feeb695cb200.png)](#challenge%20description)  
The challenge has an [attachment](https://artifacts.picoctf.net/c/472/enc_flag) for challengers to download  
  
### 
[![image](https://user-images.githubusercontent.com/70287409/228523728-4e04b686-9740-4905-bc99-aa2cfa20babb.png)](#)  
After opening the file, we can see that it is a string of encoded message. Based on the ending "==" characters, it has a high possibility to be base64 encoded  
  
__Decoding #1__  
[![image](https://user-images.githubusercontent.com/70287409/228524769-6fbaa3ba-182f-4e63-bd77-875690cd559d.png)](#)  
  
__Decoding #2__  
[![image](https://user-images.githubusercontent.com/70287409/228524892-2e449ebb-0e1f-499d-a74f-8a20f929f749.png)](#)  
  
__Decoding #3__  
[![image](https://user-images.githubusercontent.com/70287409/228524983-afb0b410-bedf-42d0-9f71-9f67191883c3.png)](#)
  
__Decoding #4__  
[![image](https://user-images.githubusercontent.com/70287409/228525212-0a6bcc29-b193-4a30-beaf-8a62cb541e80.png)](#)  
  
__Decoding #5__  
[![image](https://user-images.githubusercontent.com/70287409/228525339-8d4e046d-9fb9-4904-9834-fd6b918ab39d.png)](#)  
  
__And finally, the flag is decoded [Solved!]__  
[![image](https://user-images.githubusercontent.com/70287409/228525435-ceb6e34f-cd60-40a8-86f3-fc5486a3d342.png)](#)
  
__Note: I'm pretty sure you can run through a script to decrypt base64 until the plaintext is shown, but I'm not the best script kid out there so I'm not gonna do it :P__

<hr>  
  
## chrono  

### Challenge description
[![image](https://github.com/m4karoni/CTF/assets/70287409/9c570384-3c71-48c2-aa9c-be69b7446d63)](#Challenge%20description)  
The challenge requires the challenger to connect to the limited-time instance with ssh and provided credentials  

### chrono_t1  
[![image](https://github.com/m4karoni/CTF/assets/70287409/5fa9b30b-9faa-4088-b69c-1736ee013b00)](#chrono_t1)  
After checking with the help file from ssh, we can connect to the instance with the command:  
`ssh saturn.picoctf.net -p <port> -l <login_name>`  
[![image](https://github.com/m4karoni/CTF/assets/70287409/f1499863-27be-4b68-937c-59991c739eba)](#chrono_t1)  
First time conncting to an unknown host will be prompted wether to add the domain into known host, just type 'yes' and connect with the given password.  

I do know that cron is used to schedule tasks on Linux machine, and so I googled how to check tasks if there are any on this [website](https://phoenixnap.com/kb/how-to-list-display-view-all-cron-jobs-linux).  
### 1st command  
`crontab -l`  
[![image](https://github.com/m4karoni/CTF/assets/70287409/f41fd8dc-378b-49ca-85fc-6704be9d2e5b)](#1st%20command)  
System shows that there are no jobs... weird :\  

### 2nd command  
`less /etc/crontab`
[![image](https://github.com/m4karoni/CTF/assets/70287409/9e5acbf9-2f5e-456f-9f43-af89f4cbe3c0)](#2nd%20command)  
System does not recognise the syntax `less`  

Let's try `cat` command  
[![image](https://github.com/m4karoni/CTF/assets/70287409/3310913c-6aba-4ace-9857-121948a20195)](#2nd%20command)  
Ah ha, Just as I expected! [Solved!]  
  
<hr>  
  
##  Permissions  

### Challenge description  
<picture>
  <img title="Challenge description" src="https://github.com/m4karoni/CTF/assets/70287409/663f290c-0a1f-4524-bf8c-48710da0aa5e">
</picture>  
  
<!-- [![image](https://github.com/m4karoni/CTF/assets/70287409/663f290c-0a1f-4524-bf8c-48710da0aa5e)](#Challenge%20description)  -->
<p>The challenge requires the challenger to connect to the limited-time instance with ssh and provided credentials  </p>
