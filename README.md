# Pubmed-XML-Data-Analysis
This data science project looked at Pubmed data from a large XML file downloaded from their web page. A normalized database was designed, and the xml data was parsed, cleaned, and 
inserted into the database after hosting on on AWS. A fact table was designed to enable constant time lookup of important information one may need from the database. Rows of the fact
table include the average number of days elapsed between submission (date created in the XML) and date of publication in the journal by by year and by quarter. These are grouped by ISSN,
the unique identifier for a publisher. In the context of  a system handling millions of queries a day to extract this information, the fact table, which may only need to be updated once 
a day, can ensure fast and efficient retreival of this key information.

[R Notebook Knit](/practicum2.nb.pdf)
