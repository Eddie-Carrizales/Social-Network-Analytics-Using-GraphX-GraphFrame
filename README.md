# Social-Network-Analytics-Using-GraphX-GraphFrame
Used Spark GraphX/GraphFrame to analyze social network data for Bitcoin Alpha Platform.

## Analysis and Insights:
The social network dataset used is the Bitcoin Alpha Trust Weighted Signed Network. This is a who-trusts-whom network of people who trade Bitcoin on a platform called Bitcoin Alpha. Essentially, it’s a platform where anonymous individuals can trade cryptocurrencies without the need for an organization like a bank. Due to this anonymity, there is a necessity to maintain a record of users' reputation to prevent transactions with fraudulent and risky users.

What insights can we derive from the queries and the results we obtained?

Queries a. and b. pertain to nodes with the highest outdegrees and indegrees, indicating the nodes that are most active in initiating or receiving connections. We can observe a list of the top 5 nodes for each of these. These nodes may represent traders with a large number of connections to other traders, demonstrating their popularity within the network and frequency of trading activity.

In query c., we conduct pageranking, which essentially measures the importance of a node/trader in the network based on their connections to other nodes/traders. This can reveal the traders with the most significance or influence in the network, potentially indicating those who have a significant impact on the platform.

For query d., we identify the connected components. These components could help us identify communities of traders who interact with and trust each other.

Finally, in query e., we perform triangle counts, which represent groups of three traders who trust each other within the platform. The vertices with the largest triangle counts can also indicate traders who have a high level of engagement with each other.

Overall, conducting these queries on a social network like this allows us to identify the top traders or the most trusted traders on the platform. It also reveals relationships between traders and communities of traders who frequently trade with or trust each other.

## Instructions for running the code:
1. Sign up for a free account on Databricks Community Edition.
2. Import the notebook containing the code (.ipynb).
3. Setup/start a Spark cluster.
4. Install the included .jar file for GraphFrames
5. Execute the code.

### To install the .jar file included:
Start Your cluster -> Go to "compute" -> Click on your cluster name -> Click on "Libraries" -> Click on "Install New" -> Click on "DBFS" -> Drag the included .jar file to install.
