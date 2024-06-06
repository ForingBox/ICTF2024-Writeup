## Challenge Information

**Name**: UnDeleted

**Category**: Forensic

**Objective**: The objective of the UnDelete challenge is to recover the flag from a forensic image file. (The flag is the date of file deleted.)

# Solution
In the Challenge it provide a file named "UnDeleted".

Firstly, I go search what is .ad1 file type and what program can open .ad1 file.

From this website https://dfir.science/2021/09/What-is-an-AD1.html, i found that .ad1 file is logical images which can be open by ftk imager

So, i download the file from the challenge and open FTK imager.

After setting up FTK imager, I add the ad1 file as new evidence

![Figure 1](https://github.com/ForingBox/ICTF2024-Writeup/assets/154965035/a99fb648-eaea-4aa9-b3d8-35a3a1a2452b)

After add file into the tool, the file has a few deleted picture and others deleted files, which related to APU, BOH and FSEC SS.
![image](https://github.com/ForingBox/ICTF2024-Writeup/assets/154965035/bb5ee578-14d8-41ee-ba78-9712f280265f)

from the image above, I can see some of the files are start with $I and $R, then i go search in google.
According to this website https://medium.com/@thismanera/windows-recycle-bin-forensics-a2998c9a4d3e#:~:text=1.,deleted%20from%20the%20Recycle%20Bin. The file start with $I is store the metadata and the file start with $R is store the file's content.
![image](https://github.com/ForingBox/ICTF2024-Writeup/assets/154965035/68004157-8401-4179-848d-9782a28da20e)


## Find the flag
So, i browse thru the file list and i found a file description with the file directory "C:\Users\heehe\Downloads\flag.txt"
![image](https://github.com/ForingBox/ICTF2024-Writeup/assets/154965035/5d63946f-1021-437f-97ac-35574a92e8b3)
I found that the file deleted date and time in the properties which are 14/4/2024 10:47:50 AM



