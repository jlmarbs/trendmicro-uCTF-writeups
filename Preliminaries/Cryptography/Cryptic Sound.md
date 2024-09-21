# DESCRIPTION

We are provided with a `.wav` file and we were tasked to find the flag within that `.wav` file.

## MY PROCESS

What I initially did first is I used `QSSTV`, but then I realized when listening to the `.wav` file, it is not a radio message. So, I used `Audacity`.

After opening the `.wav` file using `Audacity`, this is what it looks like:

![image](https://github.com/user-attachments/assets/8ac44234-53d4-435c-affa-08e34a13a6c5)

Seems nothing at first. But then when I change the view into `Spectrogram`, this is what it looks like:

![image](https://github.com/user-attachments/assets/82cdb84d-3ca5-4401-86b5-cb3f7703f759)

The contents of the flag is there! But it's not really visible, so I changed the Window Size on the Spectrogram settings to `1024`.

![image](https://github.com/user-attachments/assets/28be1d16-6b91-4064-b67c-e14975a5c316)

After that I just format the contents in the flag format.

Flag: `TMCTF{TM-60999fb6-346744-09f766bd}`
