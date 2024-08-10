---
title: "PROJECT INTRODUCTION"
date: 2024-08-10
---

## Welcome

> In the inside there is sleeping, in the outside there is reddening, in the morning there is meaning, in the evening there is feeling. In the evening there is feeling.

Welcome! This is a blog documenting the Tender Buttons Project. This project usees the basic tools of data anlaysis to engage with the structure and language of Gertrude Stein's 1914 book of prose poems, *Tender Buttons*. *Tender Buttons* is in the public domain, and can be read many places, [such as at Project Gutenberg](https://www.gutenberg.org/files/15396/15396-h/15396-h.htm).

This project is: 
 - A learning exercise (think "hello world").
 - A public record that might encourage engagement with *Tender Buttons*.
 - A potential jumping off point for larger-scale, semi-automated analyses of texts, particularly performance texts. We'll see what happens! 

## The Project Plan

> A glass is of any height, it is higher, it is simpler and if it were placed there would not be any doubt. 

The project requires five steps:
1. *Text Import.* Acquire the text from somewhere.
2. *Text Cleaning.* Organize the text in a useful way.
3. *Text Export.* Move the data into a relational database.
4. *Data Analysis.* Design queries that pull meaning from the data.
5. *Data Visualization.* Display the results of the analysis. 

The plan is to iterate through these steps multiple times, refining the process and using different tools to achieve better results. Here's my plan for iteration one: 

| Stage      | Iteration One | Iteration Two | Iteration Three |
| ----------- | ----------- | ----------- | ----------- | 
| *Text Import*      | **Python.** Read the text from a local .txt file.   | TBD | TBD |
| *Text Cleaning*   | **Python.** Brute force through the text to identify and organize the words.   | TBD | TBD |
| *Text Export*   | **Python, DBBrowser for SQLite.** Export the table of words to .csv, and upload the .csv into DBBrowser. | TBD | TBD |
| *Data Analysis*   | **SQLite.** Run a battery of basic queries in an attempt to find interesting patterns. | TBD | TBD |
| *Data Visualization*   | **LibreOffice's Calc Spreadsheet.** Display the results in a static worksheet.   | TBD | TBD |

Each blog post after this one will detail the process and results of a new iteration. The idea is to not get too bogged down by mistakes and chase improvements across the board: in data accuracy, in procedural integrity, in complexity of analysis, in scalability, and in theoretical relevance. Please contact me on GitHub if you have any questions or suggestions. Thanks! 
