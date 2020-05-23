The viewpoints in the following post are my own and not meant to represent an official stance from Google.

# Spoons, Forks and Sporks
_“How you think about your customers influences how you respond to them.”_ ― Marilyn Suttle

<img src="./images/spoons_sporks_forks.png" width="600" title="Spoons, Forks and Sporks">


Data Engineers (sometimes Business Intelligence Analysts or Data Warehouse Analysts) are in the business of delivering analytics products.  As with all products, success requires setting a vision, identifying the use cases and then targeting your product to the right users.  Understanding these users is critical.  Personas are a common technique to identify personas.
Unfortunately, many personas are complex and forgettable e.g. Susan is a power user who accesses the data to update her clients who are typically mid level executives; Bob is a non-technical sales professional who wants to see his numbers in as close to real time as possible. I propose _simpler and more memorable_ personas - **Spoons, Forks and Sporks**.

## Spoons

Spoons need data delivered with softer edges and in a digestible fashion e.g. emailing a weekly operations report as a pdf, delivering a quarterly business review presentation, or sitting down for a conversation over a cup of coffee. Your client needs to be informed, but doesn't have the time, or technical skills to pull together the story themselves. Along with the data, give Spoons an interpretation. That interpretation could be a RAG (red, amber, green) status or a narrative interpretation. When possible aid them by telling them the “so what” of the report e.g. flagging things outside of expected bounds and the implications.

## Forks

Forks want to stab into the data, try out algorithm or create new metrics. You can provide the dish, but expect them to feed themselves. Give them an API, a set of tables, a HDF5 file or a S3 bucket and they are good to go. Forks will bring their own tools e.g. bash, R, python, BigQuery, etc. Your greatest service to Forks will doing the leg work up front e.g. getting the data in one place, maintain a sane data security policy, keeping a data dictionary, providing an escalation path when they want to raise questions, etc. When possible aid them by pulling all the data into a single platform to make their explorations quicker.

## Sporks

Finally, Sporks want to play with the data, but don't have the skills of Forks. Give Sporks an experience with a knobs to turn (but not code to write). An intuitive UI is the best path towards serving these users. One typical implementation could be  a dashboard with parameters to adjust product line, geography, data ranges, etc.
A single person could be classified differently in different contexts. I know many a data engineer comfortable who is a fork when it comes to web logs or big data products, but who is a spoon when it comes to finally their tax or planning for retirement.

## How do you apply this?

1. In the design and architecture phase, consider the unique needs and likely user journeys for each group. This includes documentation and training.
1. Use the terminology when discussing these groups with others.
1. Ensure you have users from each group in your User Acceptance Testing group. Each segment will capture different gaps and spot different opportunities.

