---
title: Taiwanese Mahjong Score Counter App
date: 2022-10-06T16:16:27.992Z
draft: false
featured: false
image:
  filename: featured
  focal_point: Smart
  preview_only: false
---
Taiwanese Mahjong is a 4-player game where players exchange their tiles to form a winning hand of 17 tiles. A winning hand must contain a pair and five sets of either Chows (a sequence like 1,2,3) or Pongs (three of a kind like 1,1,1). When one of the four players forms a winning hand, they would count how many scores they won from their winning hand and other players would (sometimes) pay the winner based on the score.

However, there are more than 30 scoring patterns and elements to assign scores to a winning hand. For example, one scoring element is called “Big Four Winds”, which gives the winning hand 16 points if it contains triplets of all east, south, west, and north tiles. Among those elements, some scores can be added cumulatively but some cannot. As you can see, it is very hard for new players (especially non-Chinese speakers) to know how to count scores without years of practice and memorization. It is also hard for experienced players to notice some scoring elements that rarely appear. To solve these issues, my friend (Yves Shum) and present our **Taiwanese Mahjong Score Counter**. The main functionality of this app would allow users to manually record their winning hand, and let the scores of their winning hand be counted automatically.

In our app, we use SwiftUI to build our interface, and we also load free Mahjong tile assets from Wikipedia. When a user launches our app, he will see our main page with three-button options. Two of those buttons allow users to learn Taiwanese Mahjong from external web URLs. The remaining button allows users to count scores with their winning hand. Once the users click the count score button, we enter a new view asking users to select their tiles. The app would guide users to insert their winning hand and auto-predict and auto-suggest what their hand might be. For example, when users click on OneDot for the first tile in the first set, the app would give the option of filling up the set with TwoDot and ThreeDot or two OneDot tiles. This auto feature would drastically save time for users when they insert their tiles. Once the users are done with inserting their tiles, the app would enter new views asking users to select the concealed sets*, the winning set, and the winning tile. After users select these critical elements, the app will enter the final view showing how many points users won and what the scoring elements were for the winning hand. We also implemented navigation bars on each view, so users can navigate back and forth with the views. Once the users are done with counting scores, they are able to click restart and check another hand.

\*In Taiwanese Mahjong, sets can be formed by stealing or taking another player's discarding tile (open sets) or be formed from yourself (concealed sets). Many scoring elements depend on whether sets are open or concealed.

W﻿e are aimming to upload this app to App Store and here is a [preview video](https://youtu.be/3PMM8xGXyas) of how the app looks like. I also have an inVision prototype for this work [here](https://invis.io/EQ123W3TZD3J).