---
title: Distributed Password Cracking Service
date: 2022-06-14T21:30:29.639Z
draft: false
featured: false
image:
  filename: featured
  focal_point: Smart
  preview_only: false
---
I created a distributed password cracking system. I implemented the system as a REST service and developed a client that can distribute portions of the password search space to instances of the REST service. Each call should attempt to brute force crack the password by checking each combination of letters against the hashed password. I enhanced my service to improve fault tolerance and performance by caching previous attempts. Here is my [code](https://github.com/tinghanlin/password_cracker), feel free to check it out.