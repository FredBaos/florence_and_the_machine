# Applied Dunnhumby Analysis (ADA): Discovering the Economics of Food Purchases

# Abstract
When people shop, their decisions are not purely random. Rather, people tend to keep in mind a list of items to purchase, which in turn creates an underlying economic relationships not only among products, but also between shoppers' characteristics such as income and their choices. In reality, there are challenges that tend to obscure these fundamental relationships. Retailers constantly bombard shoppers with tactics for impulse buying, let alone that people do occasionally just buy things on the fly. However, given data that spans sufficiently long time gathered from sufficiently many households, we can excavate economically relevant and intuitive consumption patterns with the right applied data analysis tools. Dunnhumby provides such a dataset with transaction records of over 275,000 unique backets of goods composed from hundreds of different commodities by more than 2,500 households in two years, which certainly offers promising opportunities to take a detailed look at interesting economics at play. In this project, we endeavor to understand how and why consumers make the purchasing decisions they do, and provide potential users with a neat, interactive network to visualize these relationships.

# Research questions
- What are some of the most frequently/rarely co-purchased products?
- What kind of economically intuitive communities arise from the co-purchase relationships among products?
- Is a household's income or number of children correlated with its consumption of certain group of products in a statistically significant way?

# Dataset
In this project, we are using the Dunnhumby dataset. We expect to use primarily the data from the demographics, products and transactions tables to answer our questions. 
As for the size of the dataset, it is very manageable: the three tables that interest us the most are less than 150 MB combined.
We only have income/children information on 801 households out of the 2500 that are in the dataset so we filtered the transactions to only keep households on which we have the information necessary to answer our questions.
We also noticed that using the price of the products instead of the quantity purchased in the transactions seems better as there are both countable items (such as loafs of bread) and uncountable items (such as gas) for which quantity has a different meaning.
There is little missing data for the description of the products so we did not have to perform a lot of preprocessing and cleaning before being able to use this dataset.

# Link to the data story
For the final report, we chose to tell a data story [online](https://fredbaos.github.io/).

# Contributions of all group members
- John: data crawling, preliminary data analysis, plotting graphs during data analysis, interactive plots for data story
- Fred: data crawling, preliminary data analysis, plotting graphs during data analysis, setting up Jekyll website, interactive plots for data story;
- Caroline: problem formulation, writing up data story, preparing final presentation;
- Frank: preliminary data analysis, plotting graphs during data analysis, design of Jekyll website, interactive plots for data story.
