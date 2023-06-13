# Too Fast
<details>
  <summary>Writeup</summary>  
  
  [![image](https://github.com/m4karoni/CTF/assets/70287409/2ebd127e-fcce-484b-bc0e-a42bbd78eea3)](#)

The challenge has given a [ctf.gif](https://github.com/m4karoni/CTF/assets/70287409/618d6c5a-c714-45f3-9ff2-d74319e1f030) file where if we download it, we can see that it's a qr code, but someone drew stuffs on it so we can't scan it properly.
  
In my experience, Photoshop is always a go to for me when dealing with gif files, and so I did.
  
[![image](https://user-images.githubusercontent.com/70287409/245427588-330bf31b-7bbe-4519-80bc-53ee1764cc1c.png)](#)  
In photoshop, these gifs are layers of different images that just repeat in a loop, so I used the Clone Stamp Tool to try to "erase" the drawings
![image](https://github.com/m4karoni/CTF/assets/70287409/a38fbd42-5d31-4c7c-b4b4-052646f95ae8)
  
After you've done it, it will be something like this  
![image](https://github.com/m4karoni/CTF/assets/70287409/9acb10aa-c0ee-4c04-ad9c-f559b63f63a9)  
It is the closest that I can do.  
It still have a little smudge on it but it's sufficient to read the qr code.
  
</details>  
  
# ow(Volume Warning)
<details>  
  <summary>Writeup</summary>  
  
[![image](https://github.com/m4karoni/CTF/assets/70287409/ac707c2a-d93b-4810-aa84-9e7eca6eae5e)](#)


Attachment: [ow.mp3](https://github.com/m4karoni/CTF/assets/70287409/aa7a8025-0219-4283-8e7a-79784962143b)  
  
**\*\*I REALLY DO NOT RECOMMEND CLICKING THE LINK BEFORE TURNING DOWN YOUR VOLUME ESPECIALLY HEADPHONE USERS\*\***  
  
For this challenge, we need to rely on some audio software, especially free ones, I recommend [Audacity](https://www.audacityteam.org/), which is an opensource audio file editor.  
  
<hr>  
When I first open up the file, it looks like this with spectogram view  

[![image](https://github.com/m4karoni/CTF/assets/70287409/09570747-533a-4c57-ac04-fd0f998d45ec)](#)  
[![image](https://github.com/m4karoni/CTF/assets/70287409/75f5cd86-1105-4f5c-b51c-808c62ff64e8)](#)  
<hr>  
But it's not what I wanted to see, so I look around the hints and it says this:  

[![image](https://github.com/m4karoni/CTF/assets/70287409/dbde982a-e9cb-4590-963f-b22201695d4d)](#)  
"What whispering," they said.  
  
I looked around on how to reduce noise in audacity and I came across this [tutorial](https://www.youtube.com/watch?v=Eyqgu4N9rho&pp=ygUraG93IHRvIGRlbGV0ZSBzcGVjaWZpYyBzcGVjdHJ1bSBpbiBhdWRhY2l0eQ%3D%3D).  
I have also stumbled upon this selection in the Effect menu. (Effect > Vocal Reduction and Isolation...)  

[![image](https://github.com/m4karoni/CTF/assets/70287409/e1f87533-3963-44ad-b974-0b79cb4a7790)](#)  
   
  <details>
  <summary>And managed to reduce unwanted noises and get the "whisper" as the flag.</summary>
  Flag: bcactf{n01s3_f4s2ph6}  
  </details>
</details>
