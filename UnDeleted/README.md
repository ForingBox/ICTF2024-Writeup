## Challenge Information

**Name**: UnDeleted

**Category**: Forensic

**Objective**: The objective of the UnDelete challenge is to recover the flag from a forensic image file.

# Solution
In the Challenge it provide a file named "UnDeleted".

Firstly, I go search what is .ad1 file type and what program can open .ad1 file.

From this website https://dfir.science/2021/09/What-is-an-AD1.html, i found that .ad1 file is logical images which can be open by ftk imager

So, i download the file from the challenge and open FTK imager.

After setting up FTK imager, I add the ad1 file as new evidence

![Figure 1](https://github.com/ForingBox/ICTF2024-Writeup/assets/154965035/a99fb648-eaea-4aa9-b3d8-35a3a1a2452b)

After add file into the tool, the file has a few deleted picture, which related to APU, BOH and FSEC SS.

