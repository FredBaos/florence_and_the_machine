# Applied Dunnhumby Analysis (ADA): Discovering the Economics of Food Purchases

# Abstract
Dunnhumby is a data science company focusing primarily on retail customer data. Inside a retail store, purchase decisions are affected by copious economic factors including the shoppers' income, how many children they have, and the way in which potentially complementary or competing products are organized and displayed. With information on the *household-level* transactions from 2,500 users over two years, Dunnhumby dataset provides ample opportunities to take the most detailed look at these interactions. In this project, we endeavor to make sense of this large dataset to understand what economic relationships are at play and provide potential users with a neat, interactive network to visualize these relationships.

# Research questions
- How can we accurately measure the degree to which products are complementary or substitutable?
- What kind of effect does household income and the presence of children have on food purchases?
- What (kind of) products are affected and in what way?
- Are there products whose consumption is not correlated with any of these factors?
- What are some known and surprising complementary and substitutable products?

# Dataset
In this project, we are using the Dunnhumby dataset. We expect to use primarily the data from the demographics, products and transactions tables to answer our questions. 
As for the size of the dataset, it is very manageable: the three tables that interest us the most are less than 150 MB combined.
We only have income/children information on 801 households out of the 2500 that are in the dataset so we filtered the transactions to only keep households on which we have the information necessary to answer our questions.
We also noticed that using the price of the products instead of the quantity purchased in the transactions seems better as there are both countable items (such as loafs of bread) and uncountable items (such as gas) for which quantity has a different meaning.
There is little missing data for the description of the products so we did not have to perform a lot of preprocessing and cleaning before being able to use this dataset.

# A list of internal milestones up until project milestone 3
- Explore other methods of measuring the relationships among products such as the correlation among quantities sold as an alternative to measuring cross price elasticities of demand. Verify if one method is more intuitive than the other.
2. Visualize the economic relationships in the form of a network. The weights of the edges can be the degree to which products are complementary/substitutable as measured by the method decided in step 1. To avoid a dense network, we plan to experiment with a few thresholds on the weight of the edges to determine what "counts" as a strong enough relationship.
3. Explore methods of comparing the similarity of the types of goods bought between households of various income level. Such a method could include Jaccard similarity.
4. Also visualize these relationships in a network (separate) where the node size can represent the income level and the weight of the edges represents the similarity in the basket of goods purchased between households.
5. Construct clusters in these graphs to see if we can create an economically intuitive groups based on these relationships. For example, we may be able to cluster dairy products and cereal products naturally from the first network, which makes intuitive sense, or identify other surprising groups. From the second network, we may be able to identify patterns in how households of similar income levels consume similar goods.
