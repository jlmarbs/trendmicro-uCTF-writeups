# DESCRIPTION

Same as the Hidden Payload challenge, we are provided with `.pcap` file and we are tasked to find the website that is being exploited if I remember correctly.

## MY PROCESS

Same with the Hidden Payload, I opened the `.pcap` file using `WireShark` and immediately looked for the `TCP` Protocol.

Once I followed the `TCP` Stream, this was the output:

![image](https://github.com/user-attachments/assets/69afccea-0170-4f0d-a2cb-c6fb9f44365c)

This challenge was relatively easy since the website was being exploited was `www.yahoo.com`.
The only weird thing of this one was, I think the flag format `TMCTF{}` was not included to the answer. 

Flag: `www.yahoo.com`

