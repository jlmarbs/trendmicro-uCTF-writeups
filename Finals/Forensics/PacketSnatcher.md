# DESCRIPTION

We are provided with a `.pcap` file and we are tasked to find the name of the image to get the flag.

## MY PROCESS

I opened `Wireshark` and immediately followed a `TCP` Stream.

This was the output:
![image](https://github.com/user-attachments/assets/f99371de-1165-4bea-9992-2dba035ef414)

![image](https://github.com/user-attachments/assets/8235a516-3920-4525-a18f-e96039e4a483)

![image](https://github.com/user-attachments/assets/7ec5e8a6-4fa8-49df-b02b-b6c8c7efe1ad)

![image](https://github.com/user-attachments/assets/3ee668a8-7346-4bdb-aca3-2adeb0ebd21f)

So there were a lot of base64 strings in the stream. And winmail.dat is not an image. What I did first is I tried decoding this part:
![image](https://github.com/user-attachments/assets/24945892-50eb-4e95-8fad-40c330d4cfb4)

When I inputted this in `CyberChef`, this was the result: 
![image](https://github.com/user-attachments/assets/a7694d4c-e9cb-45ac-a70f-fd1d42925222)

Which is nowhere near to the name of the image.

So what I did next is I tried decoding the first long base64 string:
![image](https://github.com/user-attachments/assets/b28e4d48-192e-42d0-b33e-acfc57acd3c4)

This was the result:
![image](https://github.com/user-attachments/assets/a17f956a-21d7-47d0-9b27-5c6777f4b5ea)

Scrolling down through the output, I did not see any image file. So what I did is I tried decoding again the 2nd long base64 string.

This was the result:
![image](https://github.com/user-attachments/assets/23de379c-5a73-4df5-b6ff-38e3ab429f67)

While scrolling down through the output, I saw this file name:
![image](https://github.com/user-attachments/assets/382a5d35-fd0f-4246-91e3-5770574d41d1)

We found the name of the image for the flag.

Flag: `TMCTF{info-16.png}`
