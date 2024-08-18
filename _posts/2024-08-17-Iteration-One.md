---
title: "ITERATION ONE"
date: 2024-08-17
---

*GitHub repository for Iteration One.* **ADD LINK.**

## The Basics

> All this and not ordinary, not unordered in not resembling. The difference is spreading.

In this project I'm taking the text of Gertrude Stein's *Tender Buttons* and transforming it into a form amenable to data analysis. There are many ways to do this; for this first iteration of the project, I'm starting simple. 

## 1. Text Import: Reading from a .txt

<img src="https://github.com/a-location-1/tender-buttons/blob/main/images/Tender-Buttons-Cover.png" alt="Cover page of Tender Buttons" width=50% height=50%>

##### 

The University of California libraries uploaded *Tender Buttons* to archive.org in 2007, and archive.org generates the "full text" using [some kind of optical character recognition (OCR)](https://blog.archive.org/2016/10/26/searching-through-everything/). I took [that text](https://archive.org/stream/tenderbuttonsobj00steirich/tenderbuttonsobj00steirich_djvu.txt) and copy-pasted it into local .txt files. 

It's not a perfect process: for example, page nine of the physical book is embossed with "UNIV. OF CALIFORNIA."

<img src="https://github.com/a-location-1/tender-buttons/blob/main/images/Tender-Buttons-Embossing.png" alt="Page Embossed with Univ. of California" width=40% height=40%>

Which is transcribed in the text file as this enigmatic string of characters:

```
;  y  •'  ; ;  >
```

I manually deleted them, which is really the kind of text cleaning the program is supposed to do - on to step two.  

```python
# HERE'S THE CODE FOR OPENING THE FILES.
print("Hello World")
```

## 2. Text Cleaning

My solution to (1) cleaning up the text and (2) isolating the words is to read the entire text file character by character, twice. The first pass strips out page numbers and extra spaces, the second pass builds the subsection names (which always have the same format: capital letters followed by a period, e.x. `A CARAFE, THAT IS A BLIND GLASS.`) and the words, storing the punctuation seperately.

The code tries to handle hyphens that result from line breaks, but my brute force solution isn't perfect. It also handles apostrophes (added to the word) and end punctuation (stored in a seperate variable). 

Beyond cleaning, the data needs to be arranged in a useful way so it can be turned into a relational database. I used [LucidChart](https://www.lucidchart.com/pages/er-diagrams) to make an Entity Relationship Diagram (ERD): 

![Entity Relationship Diagram with two tables, Words and Subsections](https://github.com/a-location-1/tender-buttons/blob/main/images/ERD-1.png)

In this iteration we're not actually doing any relating (I don't use the Subsections table for any analysis), but this two-table database structure lets us account for duplicate subsection names (e.x. SubsectionIDs 87, 88, 89, and 90 are all `CHICKEN.`). 

## 3. Text Export: Making a Relational database 

We did all the hard work in step two, now we just need to create an empty table to receive the data:

```sql
CREATE TABLE Subsections ( 
  SubsectionID INT NOT NULL PRIMARY KEY,
  Name VARCHAR(100)
);  

CREATE TABLE Words (
  WordID INT NOT NULL PRIMARY KEY,
  Section VARCHAR(10) NOT NULL,
  SubsectionID INT NOT NULL,
  ParagraphID INT NOT NULL,
  Name VARCHAR(25) NOT NULL,
  Punctuation CHAR(1)
); 
```

## 4. Data Analysis

## 5. Data Visualization

## Iteration Two?

>A  light  white,  a  disgrace,  an  ink  spot,  a  rosy 
charm. 

For iteration two my aim is to make my code a bit more pythonic, although I'm going to hold off on exploring some of more powerful python libraries for now. 

| Stage      | Iteration One | Iteration Two | Iteration Three |
| ----------- | ----------- | ----------- | ----------- | 
| *Text Import*      | **Python.** Import from .txt.  | **Python.** Import text from a url. | TBD |
| *Text Cleaning*   | **Python.** Manual cleaning.  | **Python.** Use objects to allow for more extensible text cleaning. | TBD |
| *Text Export*   | **Python, DBBrowser for SQLite.** Export and upload .csv. | **Python, DBBrowser for SQLite.** *Unchanged from Iteration One.*  | TBD |
| *Data Analysis*   | **SQLite.** Basic queries. | **SQLite.** Variance analysis. | TBD |
| *Data Visualization*   | **LibreOffice's Calc Spreadsheet.** Display results. | **Microsoft Excel.** Display results with sparklines. | TBD |

