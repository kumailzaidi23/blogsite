---
title: PCC - QR Recovery Challenge
date: '2024-02-01'
tags: ['ctf', 'stegnography', 'QR', 'writeup', 'forensics', 'PCC']
draft: false
summary: A hard looking challenge that was fairly very easy 
---

## Challenge Description

Maybe 0DAY?XD!!!!

![Screenshot 2024-02-05 at 2.56.49 PM.png](https://prod-files-secure.s3.us-west-2.amazonaws.com/09b77bf4-1452-421f-99f6-d0fb986688b0/8bc7c2a2-8dc0-4bd3-a106-b8b4b157bafd/Screenshot_2024-02-05_at_2.56.49_PM.png)

## Solution

This was the image that was given in the challenge, I tried to scan it with QR scanner but it was not showing any result.

![Screenshot 2024-02-05 at 2.58.06 PM.png](https://prod-files-secure.s3.us-west-2.amazonaws.com/09b77bf4-1452-421f-99f6-d0fb986688b0/c8d1822c-0e27-4c3f-b3b5-007bcea11390/Screenshot_2024-02-05_at_2.58.06_PM.png)

After reading multiple article i find out about this web tool called QRAZYBOX.

LINK: https://merri.cx/qrazybox/

After some research i find out that this is a version 5 QR code. So after opening new project and selecting blank qr code i selected the version 5.

Next was selecting the mask, for this i just select every option and checks which mask is exact match, From which i identified that Mask L 2 was perfect match.

![Screenshot 2024-02-05 at 3.03.41 PM.png](https://prod-files-secure.s3.us-west-2.amazonaws.com/09b77bf4-1452-421f-99f6-d0fb986688b0/ee62bc53-da87-4690-a3d7-8d17bfd7878a/Screenshot_2024-02-05_at_3.03.41_PM.png)

Then i start drawing the QR code here.

![Screenshot 2024-02-05 at 2.20.17 PM.png](https://prod-files-secure.s3.us-west-2.amazonaws.com/09b77bf4-1452-421f-99f6-d0fb986688b0/63699f75-114e-4e75-abcf-4a691c1d4e98/Screenshot_2024-02-05_at_2.20.17_PM.png)

After this i clicked on tools and select “Extract QR Information”

From which i got this binary

![Screenshot 2024-02-05 at 2.20.48 PM.png](https://prod-files-secure.s3.us-west-2.amazonaws.com/09b77bf4-1452-421f-99f6-d0fb986688b0/67222598-2cba-4e33-bc67-a48865eb3909/Screenshot_2024-02-05_at_2.20.48_PM.png)

Just copied this binary and convert it to ascii from this website : https://www.binaryhexconverter.com/binary-to-ascii-text-converter

Here's the flag:
![Screenshot 2024-02-05 at 2.21.08 PM.png](https://prod-files-secure.s3.us-west-2.amazonaws.com/09b77bf4-1452-421f-99f6-d0fb986688b0/6a1cd525-457a-4def-907f-f1050130c800/Screenshot_2024-02-05_at_2.21.08_PM.png)
