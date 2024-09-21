# DESCRIPTION

We are provided with the `.pcap` file and we are tasked to find the website that is used for the payload.

*(Sorry I didn't save the descriptions of the challenges :<)*

## MY PROCESS

Once I opened the `.pcap` file using `WireShark`, I immediately looked at the `TCP` Protocol since a lot of the payloads are visible on the `TCP` Protocol.

I followed the TCP Stream and this is the output:

![image](https://github.com/user-attachments/assets/7bb1763a-628f-4deb-8b9b-5eea70425595)

And there it is, the `Hidden Payload`. But it is encoded in `Base64` string, which we can decrypt using either:
- CyberChef
- `base64` Command

What I used during the challenge is the 2nd option. I copied the `base64` string and inputted this in the terminal:

![image](https://github.com/user-attachments/assets/27fd0b24-b572-45c9-84e8-d03ca6f802df)

Entering that command results to a website named `https://google.com/flags/hello_world`.
Since that was the website that the challenge is looking for, The challenge was solved.

Flag: `TMCTF{https://google.com/flags/hello_world}`
