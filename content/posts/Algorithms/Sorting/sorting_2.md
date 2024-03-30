---
title: "Sorting Problem"
subtitle: "with java"
date: 2024-03-30T17:20:00
lastmod: "2024-03-30"
description: "Let's learn how to sort data"
categories: ["Algorithms"]
series: ["Sortng"]
tags: ["Algorithms", "Problem", "Sorting"]
image: "/images/default.jpg"
draft: false
hideFromHomePage: false
math: false
mermaid: false
---

# Problem

Jay likes sequences, so he use to playing with a sequence of size N. He will transform the sequence according to K queries, and the format and process of the queries are as follows:  

- L R X: Let's say the sequence sorted in ascending order is A[1], A[2], …, A[N]. 
- First, add X to A[L], A[L+1], …, A[R]. 
- Then, sort the sequence again in ascending order.  
   
Print the sequence after performing all the queries in order.
<!--more-->

## Input  


> tip
> The first line is given with N and K separated by a space. (1 ≤ N ≤ 100000, 1 ≤ K ≤ 1000)  
> The second line is given with N integers that make up the sequence, each having an absolute value of less than or equal to 10^18.  
> From the third line to the (K+2)th line, the queries L R X are given. (1 ≤ L ≤ R ≤ N, |X| ≤ 10^9)


## Output  


> tip
> Print the sequence after performing all the queries in order.

---
# How to Approach?  

