# Applied Dunnhumby Analysis (ADA): Discovering the Economics of Food Purchases

# Abstract
Dunnhumby is a data science company focusing primarily on retail customer data. Inside a retail store, purchase decisions are affected by copious economic factors including the shoppers' income, how many children they have, and the way in which potentially complementary or competing products are organized and displayed. With information on the *household-level* transactions from 2,500 users over two years, Dunnhumby dataset provides ample opportunities to take the most detailed look at these interactions. In this project, we endeavor to make sense of this large dataset to understand what economic relationships are at play and provide potential users with a neat, interactive network to visualize these relationships.

# Research questions
- How can we accurately measure the degree to which products are complementary or substitutable?
- What kind of effect does household income and the presence of children have on food purchases?
- What (kind of) products are affected and in what way?
- Are there products whose consumption is not correlated with any of these factors?
- What are some known and surprising complementary and substitutable products?
- How can we represent these economic relationships in the form of a graph?
- Can we construct clusters in this graph which are intuitive economically and come naturally from these relationships?

# Dataset
We want to use the Dunnhumby dataset. We expect to use primarily the data from the demographics, products and transactions tables to answer our questions.
We only have income/children information on 801 households out of the 2500 that are in the dataset so we plan to filter the transactions to only keep households on which we have the information necessary to answer our questions.
We also noticed that using the price of the products instead of the quantity purchased in the transactions seems better as there are both countable items (such as loafs of bread) and uncountable items (such as gas) for which quantity has a different meaning.
There is little missing data for the description of the products so we don't expect a massive amount of preprocessing and cleaning for this part of the dataset.
As for the size of the dataset, it is very manageable: the three tables that interest us the most are less than 150 MB combined.

# A list of internal milestones up until project milestone 2
- Get more familiar with the dataset
- Filter / clean / sanitize the different tables we want to use
- Setup a pipeline to compute the statistics that interest us (such as product income elasticity, product complementarity, ...)
- Perform some basic visualization to check that our results make sense
- If necessary (some results hard to explain) augment the transaction data with direct advertising information (such as the coupons sent to households or the way some products are favorably displayed in the stores) and see if that explains unexpected results

# Questions for TAs
So far we do not have any questions for TAs.
