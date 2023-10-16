# Two Articles about Graph Databases

Welcome! In this document, I discuss two articles introducing a fancy type of database: the graph databases. I summarize what the authors talked about and share my thoughts.


## first article

Source: Favio Vázquez's [Graph Databases. What’s the Big Deal?](https://towardsdatascience.com/graph-databases-whats-the-big-deal-ec310b1bc0ed)

The article provides a good overview of the benefits of using a graph database versus a traditional relational database. I think the key advantage highlighted is how a graph database allows you to efficiently query interconnected data by leveraging the relationships between entities. This is perfect for use cases like social networks, knowledge graphs, and fraud detection where you need to analyze connections.

My main takeaway is that graph databases shine for highly linked data where relationships matter. The graph structure of nodes and edges maps well to querying relationships. While relational databases can also model some connections through foreign keys, traversing these connections requires multiple join operations which get inefficient at scale. Graph databases make it easy through their optimized data model.

However, I do think that there are still challenges and limitations around properly modeling certain types of data for graph databases compared to mature relational databases. For many use cases, a relational database may still be a better choice. But for highly interconnected data, graph databases provide optimization that is difficult to achieve otherwise. Overall, it's beneficial to understand both technologies and when each one is better suited.


## second article

Source: Neo4j's [Graph Databases for Beginners: Why Graph Technology Is the Future](https://neo4j.com/blog/why-graph-databases-are-the-future/)

This article makes a strong case for the power of graph databases and why interconnected data is becoming increasingly important. I agree that relationships are crucial for many emerging use cases like personalized recommendations, fraud detection, and knowledge graphs. Modeling these connections efficiently is critical.

However, I think the article goes too far in claiming graph databases will completely replace relational databases. The reality is that both serve important but distinct purposes. Relational databases are better for transactional data and strong consistency needs. Graph databases optimize for flexibility and traversing relationships. The article downplays the challenges of migrating existing systems and tools to an entirely new paradigm.

The best approach is to use the right tool for the job. Graph databases clearly excel at graph problems like traversing social connections. But many datasets are still better modeled in a tabular relational structure. A hybrid solution combining both relational and graph technologies is likely optimal for many complex needs. While graph databases will continue growing in popularity, it’s an overstatement to claim they will completely take over. The world still has many tabular and transactional data needs that relational handles well. But for connected data, graph databases provide invaluable relationship modeling that can’t be beat.
