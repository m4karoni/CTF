# General Skills

A category where you typically Google your way to get your flag  
  
## Contents
- [money-ware](#money-ware)
- [repetitions](#repetitions)
- chrono
- Permissions
- useless
- Special

<hr>

### money-ware
[![image](https://user-images.githubusercontent.com/70287409/228513250-dec6565b-088d-4c0b-be48-0b28a8697502.png)](#)  
The challenge was to find the name of the Malware and the description gave us some hint about some Bitcoin wallet address `1Mz7153HMuxXTuR2R1t78mGSdzaAtNbBWX`  
  
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
  
### repetitions  
[![image](https://user-images.githubusercontent.com/70287409/228523307-1fb5e100-e53a-4afe-8755-feeb695cb200.png)](#)  
The challenge has an [attachment](https://artifacts.picoctf.net/c/472/enc_flag) for challengers to download  
  
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
