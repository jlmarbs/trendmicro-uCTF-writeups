# DESCRIPTION

We are provided with a `.wav` file and we were tasked to find the flag within that `.wav` file.

## MY PROCESS

What I initially did first is I used `QSSTV`, but then I realized when listening to the `.wav` file, it is not a radio message. So, I used `Audacity`.

After opening the `.wav` file using `Audacity`, this is what it looks like:
![[Pasted image 20240922000124.png]]

Seems nothing at first. But then when I change the view into `Spectrogram`, this is what it looks like:
![[Pasted image 20240922000207.png]]

The contents of the flag is there! But it's not really visible, so I changed the Window Size on the Spectrogram settings to `1024`.
![[Pasted image 20240922000334.png]]

After that I just format the contents in the flag format.

Flag: `TMCTF{TM-60999fb6-346744-09f766bd}`