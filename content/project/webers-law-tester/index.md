---
title: Weber's Law Tester On Vision
date: 2021-10-17T06:03:15.789Z
draft: false
featured: false
tags:
  - python
image:
  filename: featured.png
  focal_point: Smart
  preview_only: false
---
I designed a Weber's Law Tester on vision. **Weber’s law**, also called **Weber-Fechner law**, is historically important psychological law quantifying the perception of change in a given stimulus. The law states that the change in a stimulus that will be just noticeable is a constant ratio of the original stimulus. It has been shown not to hold for extremes of stimulation.

I used python to design this interactive Weber's Law Tester. Once a player runs my testers, the terminal prompts will ask you to pick which subplot has more dots. The player will need to "Press 1 if the left subplot has more dots" or "Press 0 if the right subplot has more dots". The player will only have 1 second to answer each question. My program contains 10 mini sections. It will take a player around 2 minutes to to complete all 10 sections. In the end, my program would show the player's study result. For example, "You are able to tell which subplot has 20 dots, when the difference between the number of dots is around 2.5 dots".

Here is my [python code](https://github.com/tinghanlin/webers-law-tester) for my interactive program! Notice that my code is adjusted to Python 3.x, so make sure you have the right environement to run the code. Feel free to download my folder, and run “*python webers-law-tester.py”* in my folder and see if your vision conforms with Weber's Law!