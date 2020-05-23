The viewpoints in the following post are my own and not meant to represent an official stance from Google.

Problems with Spreadsheets for Analytical Work

I am contrasting Spreadsheets with Python, but other suitable analytical languages exists e.g. R, Julia.

## Meaningless Cell References  
- E.g. A cell this formula`= B4 + E6`. What do B4 and E6 represent?
- Made worse when the cells are pulled from other sheets or other spreadsheets.
- Yes, you can name cells. How many of you do it?
- Python 

## Overloaded Cells 
- Cells could be names, descriptions, units, formulas, and values! 
- 3 Dogs. $ 256.35.  =B4 + E6. "States". Can lead to QA issues or confusion.

## No separation between Code and Interface
- You share your spreadsheet, You share your code. 
- Limits commercial market. 

## Invisible Dependencies
Trace Dependencies on Excel kinda works... on a PC. 
But still no concept of breakpoints. Cntrl ~ is hard to read.

## Poor MultiUser Support and Syndication 
- Google Spreadsheets is exception. 

## Joining Datasets is Clunky
- Vlookup. Messy to do multiple columns. Who likes mixed references? VLookup must be copied for every cell (not smart enough to handle multiple values) 

## Lack of looping capabilities
- Spreadsheets do have 

## Versioning is challenging
- Version 
- Version 23. Version 24. A Quick Story (nothing proprietary!). 

## Diffing files is very challening
- Excel uses OOXML to store the data. The OOXML spec is 7,000 pages. 
- ODF format is 'only' 500 pages. Good luck versioning that!

## Lack of Modularity
- Hey Bob, you created that nice segmentation model for repeat customers. 
- Can I borrow a piece of it for my project? 
- Difficult to consolidate the work of multiple people together.


## Hard to get the Data Out 
- Sometimes our work gets shared downstream
- Pulling data from a spreadsheet is precarious. Users may move columns, skips rows, etc.
- Each of those changes risk that downstream process pulling in incorrect information.

## Confusing Copying Behavior
- Copying cells with fixed references (i.e. $) is different, but not obvious

## Difficult to test
- If you are doing complex calculations then you often want to test those calculations
- Programming languages like Python allow you to create unit tests.
- Minimal unit tests capabilities

## Not suited for continuity
- People change jobs. Someone else has to pick 
- No accepted style guide. Contrast with PEP 8.
