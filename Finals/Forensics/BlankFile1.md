# DESCRIPTION

We are provided with a `.zip` file. We are tasked to find the flag within the `.zip` file.

## MY PROCESS

When I unzipped the `.zip` file and check what file type the extracted file is, this is the output:

![image](https://github.com/user-attachments/assets/833792d8-6bd7-4a26-8c3f-2d60446f6a13)

So what I did is that I renamed the file to have the `.xlsx` extension and opened the file.

This was the result when I opened the file:

![image](https://github.com/user-attachments/assets/f046dacb-e6b9-4467-91ea-35531be77b52)

It was literally a blank file. So what I did afterwards is I used `binwalk` to check for some files that are embedded to the excel file, and this was the result:

![image](https://github.com/user-attachments/assets/7802f98d-527f-4e26-bb50-46dcd2ac1613)

There was indeed a `.zip` file embedded to the excel file. What I did after is I extract those files.

This is where I trial and error stuffs. *(going through directories and reading the .xml files)*

Then I stumbled upon `xl/` directory. After that I tried reading the `sharedStrings.xml` file and this is the output:

![image](https://github.com/user-attachments/assets/9e993407-9dab-4c41-9e91-3832cde5a21e)

I noticed that the flag is there but is being broken down into chunks. So what I did is that I formatted the flag in the notepad.

Flag: `TMCTF{Bl4deRunn3r}`
