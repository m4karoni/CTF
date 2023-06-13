## Dots and Dashes
<details>
  <summary>Writeup</summary>  
    
  ![image](https://github.com/m4karoni/CTF/assets/70287409/e0ee2fde-f575-4195-94f3-09b47fcae6c5)  

  [code.txt](https://storage.googleapis.com/bcactf/dots-and-dashes/code.txt)  
    
  This text file consists of dots and dashes like the title, but it is no ordinary dots and dashes.  
  I tried to decode it as Morse code but it didn't work, because there were no spaces in between words.  
    
  So I decided to go look for the hint 
  
  ![image](https://github.com/m4karoni/CTF/assets/70287409/4621d613-d61a-44de-b586-e7f40b69fdde)  
  "What other codes only use 2 chracters?" they said.  
  
  I googled the exact phrase and got and idea from the result I saw: Binary  
  So I translated the dots as 0 dashes as 1 with python script and got nothing.  
    
  ```py
  f = open("code.txt","r")

  t = f.readline()

  txt = t.replace('.','0').replace('-','1')

  n = 8

  code = ' '.join([txt[i:i+n] for i in range(0,len(txt),8)])

  # adding spaces in between 8 characters
  
  print(code)
  ```
    
  ![image](https://github.com/m4karoni/CTF/assets/70287409/4a5f2c0b-73be-43fe-b866-a95d58dee985)  
  
  ```py
  f = open("code.txt","r")

  t = f.readline()

  txt = t.replace('.','1').replace('-','0')

  n = 8

  code = ' '.join([txt[i:i+n] for i in range(0,len(txt),8)])

  print(code)
  ```
    
  <details>
    <summary>So I turned the replacing around and translated it again, and got this </summary>
      
![image](https://github.com/m4karoni/CTF/assets/70287409/b73e73ab-70a8-4b9f-bb21-14c64dbd72d5)

  </details>
  
</details>
