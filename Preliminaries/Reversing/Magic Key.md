# DESCRIPTION

We are provided with a `MagicKey.txt` and we were tasked to find a website in the `.txt` file itself *(If I remembered it correctly)*

## MY PROCESS

Upon checking the `.txt` file itself, it has 1998 lines in the `.txt` file.

![image](https://github.com/user-attachments/assets/0d74e868-990d-4048-8613-7f45f562d621)

When I opened the `MagicKey.txt` file, this was the contents:

```
2F396A2F34414151536B5A4A52674142
41514541654142344141442F34524461
525868705A674141545530414B674141
41416741424145374141494141414146
41414... it's so long...
```

For me it looked like a `Hex Strings`.

So what I did after is I went to `CyberChef` and basically put the `From Hex` operation.

![image](https://github.com/user-attachments/assets/7b6260fe-fa34-4922-853c-75cfbcc2d2ce)

Checking the output, it tells me that this was also encoded in `base64`. So, I added the `From Base64` operation.

![image](https://github.com/user-attachments/assets/99b3a765-d989-4906-8ffd-9d4e14e2bb5d)

Now we are getting somewhere with the file header being `JFIF`. This means we can basically convert that into an image.

So what I did is I added `Render Image` operation in `CyberChef` and long behold:

![image](https://github.com/user-attachments/assets/56a11e86-d206-4845-a894-b548fbcf3977)

There is the website we are looking for.

Flag: `TMCTF{www.thisis3t.com}`
