# Build

## Process

1. Project tracking
    1. Meetings - Normal enginer meetings are not a fit.
    1. Bugs - 
    1. Regular comms - Highlights, lowlights, past week review, 


## Tool

Three tools often come up

1. Spreadsheets
1. Notebooks
1. Code

### Spreadsheets

In general development is spreadsheets is discouraged behind explorary data analysis or quick proofs of concept. See "Problems with Spreadsheets"

### Notebooks

Jupyter notebooks have become a common environment for analysis. Notebooks combine together handy features for development (inline charting, markdown, magic functions, etc). However notebooks lack features for producing modular code and enabling peer review.  Notebooks suffer from cruft
  1. Cruft from the state of the notebook. Code can be executied in arbitrary order of cells. And the results stored in the notebook.
  1. Cruft from extra cells.
  1. Difficult peer review
  1. No standard unit test mechanism.

Notebooks have a central role to play in analytics, however for mature projects any notebook elements that benefit from:

  1. Reuse. Do you expect the code to be reused across multiple projects.
  1. Complex data manipulations or calculations.
  1. Long running code. Are you running code in production for multiple quarters? 

If your project mets any of the above criteria then you should check in the core parts of the project into source control.

### Code

Python readability standards followed. Function signatures should align to sklearn i.e. initiate, fit, analysis. If python readability is not present on the team then starting with experimentals directories allows most of the benefits and is good practice for developing readability.

> TIP: Creating a unit test for analytical code. 
> Unit tests for analytical code provides two benefits - ensures the quality of functions and ensures the quality of the the analysis. Test manufactured data e.g. perfectly linear data, data with extreme values. 
> - This manufactured data should deterministically produce a known results e.g. significant p value, all zero matrix.
> - Use UnitTest's setup features to create the sample data. Here is a receipe where fake csv data is loaded.
> - What about system testing? Typically an analytical project will fit into a larger system or data flow. That is the level where system testing should live.
> - For sizable projects code should be broken up into (1) Import (2) Manipulations (3) Analysis. This is especially handy when the import or manipulation is large and time consuming. 
> - When possible code should be idempotent.

## Documentation

- Markdown
  - Same location as code. No worries about file permissions. 
  - Disadvantage that not are pretty for users. 
- Slide decks are useful for users.
- Recommendation: Build a slide deck that succiently represents the work. But keep the majority of the documentation with the actual code of the project. See "Read the docs" or "SciKit Learn".