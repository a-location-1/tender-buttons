---
title: "PROJECT INTRODUCTION"
date: 2024-08-10
---

## Welcome

> In the inside there is sleeping, in the outside there is reddening, in the morning there is meaning, in the evening there is feeling. In the evening there is feeling.

Welcome! This is a blog documenting the Tender Buttons Project. This project uses the basic tools of data analysis to engage with the structure and language of Gertrude Stein's 1914 book of prose poems, *Tender Buttons*. *Tender Buttons* is in the public domain, and can be read many places, [such as at Project Gutenberg](https://www.gutenberg.org/files/15396/15396-h/15396-h.htm).

This project is: 
 - A learning exercise (think "hello world").
 - A public record that might encourage engagement with *Tender Buttons*.
 - A potential jumping off point for larger-scale, semi-automated analyses of texts, particularly performance texts. We'll see what happens! 

## Why Tender Buttons?

Modernist writing has a reputation for difficulty; data analysis is a way to approach modernist texts from a different angle. 

In a 1946 interview Stein described the process of writing *Tender Buttons*: "I used to take objects on a table, like a tumbler or any kind of object and try to get the picture of it clear and separate in my mind and create a word relationship between the word and the things seen. [...] I try to call to the eye the way it appears by suggestion the way a painter can do it. This is difficult and takes a lot of work and concentration to do it. I want to indicate it without calling in other things."[^1] 

*Tender Buttons* is a product of tremendous attention, making it a perfect candidate for sustained analysis. It's also serendipitous that "tender buttons" sounds like one of GitHub's randomly generated names for a new repository - the legacy of modernism in contemporary form. 

###### Damien Elwes, *Picasso's studio at Bateau Lavoir 1908* (2010).[^2] Robert Bartlett Haas writes that "*Tender Buttons* was to Gertrude Stein's development what the "Demoiselles d'Avignon" was to Picasso's, a key work marked with the enormous struggle of creating a new value."[^3]

This is test text. 

![DamienElwes2010]({{site.url}}/images/DamienElwes2010.png?raw=true)

![DamienElwes2010](images/DamienElwes2010.png?raw=true)

![DamienElwes2010](images/Damien-Elwes-2010.png.png)

![DamienElwes2010](/images/Damien-Elwes-2010.png.png)

![DamienElwes2010](./images/Damien-Elwes-2010.png.png)

![DamienElwes2010](../images/Damien-Elwes-2010.png.png)

![DamienElwes2010](DamienElwes2010.png)

![DamienElwes2010](images/DamienElwes2010.png)

![DamienElwes2010]({{site.url}}/images/DamienElwes2010.png)

![DamienElwes2010](https://github.com/a-location-1/tender-buttons/blob/main/images/DamienElwes.png)

<img src="https://github.com/a-location-1/tender-buttons/blob/main/images/DamienElwes.png" style="margin: auto;" />

<img src="{{site.url}}/images/DamienElwes2010.png" style="margin: auto;" />

<img src="{{site.url}}/images/DamienElwes2010.png" style="margin: auto;" />

<img src={{site.url}}/images/DamienElwes2010.png margin: auto />

<img src={{site.url}}/images/DamienElwes2010.png alt=DamienElwes2010 width=auto align=left />

<img src={{site.url}}/images/DamienElwes2010.png margin: auto >

<img src={{site.url}}/images/DamienElwes2010.png margin=auto >

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

Each blog post after this one will detail the process and results of a new iteration. The idea is to avoid getting bogged down by mistakes and chase improvements across the board: in data accuracy, in procedural integrity, in complexity of analysis, in scalability, and in theoretical relevance. Please [contact me on GitHub](https://github.com/a-location-1) if you have any questions or suggestions. Thanks! 

[^1]: "A Transatlantic Interview--1946." *A Primer for the Gradual Understanding of Gertrude Stein.* Ed. Robert Bartlett Haas. Black Sparrow Press, 1971. 

[^2]: Detail from Damien Elwes, *Picasso's studio at Bateau Lavoir 1908* (2010). Printed in Baiges, Maite Méndez. "After Picasso: Reinterpretations and recreations of *Les Demoiselles D'Avignon* in Contemporary Art." *Les Demoiselles d'Avignon and Modernism.* Firenze University Press, 2022.

[^3]: "A Transatlantic Interview--1946."  
