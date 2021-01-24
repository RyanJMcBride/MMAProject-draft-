# MMAProject
The aim of this project is to answer the question "How often can does 'MMA math' work in the UFC?"

More specifically the question is asking, "Do mma matches exhibit a transitive property". Moreover, if
A,B & C are fighters and A>B indicates that A defeated B, then how often is the following logic consistent:

A>B and B>C does that mean A>C?

If A>C, then MMA math 'works' for this particular case and vice versa.

To get a quantitative answer, ufc fight data is collected and a ratio of of (mma math works)/(mma math works + doesnt)
is calculated.

The steps involved are as follows:
1. Using python's BeautifulSoup and Requests packages, scrape ufcstats.com to obtain a dataset of all past mma fights
and export the dataframe to a csv.
2. Load and transform the data into a dictionary of fights for each ufc fighter using Pandas library.
3. Create an algorithm that finds all possible 3 fight sequences where fighters A,B & C have fought eachother.
4. Determine percentage of fights where the transitive property holds

