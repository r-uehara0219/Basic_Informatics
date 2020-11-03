# week01 -Processing of Information(1)-
1. Explain what databases and database management systems are.  
Database is a collection of large amounts of data, organized in a way that makes it easy to add, delete, and search data on a computer. Database management system is a software that serves as an interface between users and the database and manages the database efficiently and appropriately.

2. Explain the ACID criteria of databases.  
The ACID criteria of databases is an acronym for four properties that summarize the properties that transactions in a reliable database should have. Atomicity is the property that the sequence of operations contained in a transaction is guaranteed to be either executed as a whole or not executed. Consistency is the property that processing is performed in accordance with the rules specified in advance. Isolation means that for a process, only the data before and after execution can be seen from the outside, and the state of the data during execution cannot be seen. Durability is the property that when a process is completed, its output is recorded in the database as not being lost permanently.

3. A relational database consists of a set of relations. Use an example to explain key elements of a relation in relational databases.  
For example, consider a case where there are two tables: an "Employee table" and a "Department table". In the "Employee table", each employee's department is assigned by a number, and in the "Department table", the name and location of the department corresponding to the number are entered. By managing them separately, even if one department is moved to another branch, the data in the "department table" can be changed only by one change.

4. Briefly describe the procedure of the database design.  
The database design phase can be divided into three main phases: conceptual design, logical design, and physical design. Conceptual design extracts the data needed to perform the tasks that require a database and creates a "conceptual data model". In logical design, a "logical data model" is created by organizing the conceptual data model and transforming it into a form suitable for the type of database used. Physical design not only ensures the necessary hardware resources and determines the physical data placement, but also organizes the database with performance considerations to create a more realistic "physical data model.

5. Explain the key concept of the entity relationship model.  
Entity Relationship is a blueprint for organizing data in a database. In the ER diagram, the group of data that makes up the database is represented by a rectangle called an "entity". The data is then connected to each other by a line called a "relationship" and a notation called "cardinality" is used to indicate the relationship between them.

# week 2 -Processing of Information(2)-
1. Explain the role of database keys in relational database management systems.  
A foreign key in a relational database is used to ensure that one column of a table can only be filled with items that are contained in a particular column of another table.

2. Give an example of a relation in relational databases and specify its primary key.  
Consider the case of designing an "employee table" and a "department table". The relationship is established by adding a column of "Department Code" to the employee table and associating it with "Department Code" which is the primary key of the department table.

3. Explain what the following operations do in relational databases. Use examples if necessary.
Selection is an operation to select a row in a table. In SQL statements, use SELECT statements.
Join is an operation to make one table from multiple tables.
A Cartesian product is one that takes the elements of each table, one by one, and thinks about all the combinations.

4. Explain the meaning of database normalization.  
Database normalization is the process of organizing the data so that there are no inconsistencies when updating it. It involves creating tables according to rules designed to protect data and establishing relationships between those tables, as well as increasing database flexibility by eliminating redundancy and inconsistent dependencies.


# week3 -Processing of Information(3)-
1. Explain the difference between structured data, semi-structured data, and unstructured data.
       Structured data uses the "Schema-on-Write" method, in which the structure for managing data is decided in advance and data is stored according to the structure. It is used to manage data within a specific scope, such as each company, and is implemented in RDBMS.
       Unstructured data has no fixed format or content, and includes any data that can be collected through the Internet or other means.
       Semi-structured data is defined as giving unstructured data a flexible structure. Semi-structured data has symmetrical characteristics to structured data. The data is stored with tags according to the data collected, and the data is applied to the data structure in the form that you want to use when you want to use it. It allows us to handle a wide variety of data, which is also characteristic of unstructured data, and is implemented in NoSQL databases.

2. Explain what XML is and what it is used for.  
XML is a markup language for describing the meaning and structure of documents and data. It is mainly used to simplify the exchange and management of data.

3. Explain the difference between HTML and XML.  
While HTML is used to decorate web pages, XML is used to describe data, such as to make data in a document easier to understand or to exchange data.

4. Describe the advantages of XML.  
    First, XML makes it easy to understand the meaning of data. Feel free to define element names according to the meaning of the data to make the data stand out clearly.
    Secondly, it is highly scalable. It is suitable for the management of data, because the data structure such as element names can be freely defined.
    Third, it can be adapted to any computer system. Since the description method is standardized in the world standard, it can be applied to any computer system by converting data into XML, which makes it easy to share and disclose information.

5. Explain what DTD (Document Type Definition) is.  
DTD is a definition file that defines how to write XML, HTML, etc. DTD can define tags to be used in a xml file, attributes that can be used with those tags, and entity references.

# week4 -Search and Management of Information(1)-
1. Explain what information retrieval is based on your own understanding.  
Information retrieval is the process of retrieving the desired item from a large amount of information in a short period of time.

2. Describe the search process by using search engines (e.g., Google).  
Google organizes its content on the web in advance using a search index. As users type keywords into the search window, the search algorithm is set in motion and a huge number of Categorize web pages to find the most relevant ones.

3. Discuss the differences between database systems and information retrieval systems.  
Database systems only stock information in predetermined fields, whereas information retrieval systems can retrieve information in a wide range of fields.

4. Query is a representation of user search intent in information retrieval. Give three examples of query types in information retrieval systems.  
    Firstly, there is the informational query. This is a query that users set up to find out what they want to know. For example, "KyotoUniversity location" is an example of this.
    Secondly, there are transactional queries. This query is set up when users want to take action. For example, "Kyoto hotel reservation" is an example of this.
    Third, there is a navigational query. This query is set up when a user wants to access a specific site. For example, "KyotoUniversity PandA" is an example of this.

5. Explain what Web crawlers are and how Web crawling is conducted.  
    A web crawler is a program that automatically collects text, images, videos and other information published on the Internet and stores it in a database.
    The crawler accesses and parses web pages. It processes the information on the page and converts it into data that is easy for search algorithms to handle, and also add the link to the database.
    When a link is found by analysis, the crawler jumps to the link, analyzes the information collected on the linked page and registers it, and repeats the process.

# week5 -Search and Management of Information(2)-
1. Explain the concept of inverted indexes. Use an example if necessary.  
An inverted indexes is index to increase the speed of text search. The inverted indexes divides the contents of each document into words and uses them as keys. Then, sentences in which the word appears are placed in the value.

2. A search query is usually composed of several terms that reflect users’ information needs. Describe the process of search using inverted indexes.
For example, if we use inverted indexes for the search query "Tokyo mosque",
```
Pages containing "Tokyo":
・University-of-Tokyo.net
・Tokyo-Camii.net
・Tokyo-Disneyland.net
```
```
Pages containing "mosque": 
・Sultanahmet-Camii.net
・Tokyo-Camii.net
・Umayyad-Mosque.net
```
("Camii" is synonymous with "Mosque")  
We can get a list of pages containing each term as follows. By taking these summation sets, the page "Tokyo-Camii.net" containing the two words "Tokyo mosque" can be quickly Searchable.

3. Explain what biword indexes and positional indexes are, respectively.  
Biword indexing is splitting a query into two terms each and treating them all as phrases. For example, if there is a query "A B C D", it is converted to 'A B' && 'B C' && 'C D'.
Positional indexes are Biword indexes plus information on occurrences.

4. Explain the concept of term frequency-inverse document frequency (TF-IDF).  
TF is the frequency with which a word appears in a document. The more often a word appears in a document, the more likely it is to be important.
IDF is the inverse of the document frequency in which a word appears. A word that appears in many documents is unlikely to be the feature word of a single document.
The TF-IDF is a method that combines these words to find the characteristic words of a document.

# week6 -Search and Management of Information(3)-
1. Explain the following concepts in graph theory: (a) graph, (b) degree of a vertex, and (c)weighted graph.  
1-1. A graph is an abstract data type consisting of vertices and edges that represent the connectivity between them. It is used to describe the structure of the combination.  
1-2. The degree of a vertex is the number of edges coming out of the vertex.  
1-3. A weighted graph is a graph with weights attached to the edges of the graph.

2. First, briefly describe the basic idea of PageRank. Then, explain the PageRank algorithm in detail, in no less than 200 English words.  
Page Rank is one of the web page evaluation metrics in Google search engine. It ranks web pages on an 11-point scale of "0-10" based on their links. In theory, a PageRank score could be calculated by someone randomly linking to each website by This is the extreme probability that you will end up on a specific page by clicking on it.
   PageRank assumes a "random surfer" model. First, all start by randomly selecting the first page. Secondly, those who stay on one page will be moved to another page in the next time slice. Third, the pages with the highest probability of staying are ranked as useful pages.
  The PageRank algorithm creates a Markov chain model for the above random surfer and uses The idea is to create a ranking by finding the transition probability of the steady state. A Markov chain model is a stochastic process with Markovian properties. ('Markovian' refers to the property that the conditional probability distribution of future states depends only on the present state. "Stochastic process" refers to a stochastic variable that changes over time.)
   Applying this method has the effect of reducing the relative importance of sites that are just linking to each other among their peers, and reducing the importance of links from sites that are just linking to each other, such as many links.

3. Explain the function of the damping factor in PageRank.  
The damping factor is a parameter that adjusts the influence of the importance of the link to be linked. It is usually set to 0.85. A site that is trying to artificially increase its page rank will have a low dumping factor.

# week7 -Search and Management of Information(practice)-
[Question 1]

Consider these documents:

Doc 1    breakthrough drug for schizophrenia 
Doc 2    new schizophrenia drug 
Doc 3    new approach for treatment of schizophrenia 
Doc 4    new hopes for schizophrenia patients

Draw the term-document incidence matrix for this document collection.
Draw the inverted index representation for this collection.

[Answer 1]

|    |               | Doc1 | Doc2 | Doc3 | Doc4 |
|----|---------------|------|------|------|------|
| 1  | approach      | 0    | 0    | 1    | 0    |
| 2  | breakthrough  | 1    | 0    | 0    | 0    |
| 3  | drug          | 1    | 1    | 0    | 0    |
| 4  | for           | 1    | 0    | 1    | 1    |
| 5  | hopes         | 0    | 0    | 0    | 1    |
| 6  | new           | 0    | 1    | 1    | 1    |
| 7  | of            | 0    | 0    | 1    | 0    |
| 8  | patients      | 0    | 0    | 0    | 1    |
| 9  | schizophrenia | 1    | 1    | 1    | 1    |
| 10 | treatment     | 0    | 0    | 1    | 0    |

 

drug: “Doc1”, “Doc2”

new: “Doc2”, “Doc3”, “Doc4”

schizophrenia: “Doc1”, “Doc2”, “Doc3”, “Doc4”


# week8 -Analysis of Information(1)-
1. Explain what machine learning is, based on your own understanding.  
Machine learning is the process of learning patterns in large amounts of data to acquire a model for determining unknown data.

2. Describe the differences between supervised learning and unsupervised learning.  
Supervised learning is a type of learning where there is a correct answer and the algorithm is expected to predict such an answer. thing.

    Unsupervised learning does not refer to labeled results, but rather to groups of common characteristics from the data. Learning to find or extract structures and patterns in data.
 
3. Explain the Naïve Bayes Classification method and the KNN Classification method, in no less than 300 English words in total.  
Naive Bayesian classifier is a method that uses Bayes'theorem to calculate the probability of being classified into each class and outputs the class with the highest probability as the result.

    The KNN classification method is a method that plots the training data on a vector space, and once the unknown data is obtained, arbitrary Ks are obtained from it in order of distance, and the class to which the data belong is estimated by majority vote.

4. Explain the purpose of n-fold cross validation and how it is conducted.  
n-fold cross-validation is the process of splitting the sample data, analyzing a portion of it first, and then using the remaining portions of the A method of testing the analysis and applying it to confirm the validity of the analysis itself. The purpose is to prevent bias in the trainer by crossing data for training and data for verification.

# week9 -Analysis of Information(2)-
1. Describe a basic algorithm for decision tree learning, in no less than 200 English words.  
Decision tree learning is an algorithm that searches for the "leaf" that best matches the conditions by tracing the branching from the "root".
Based on the training data, a conditional expression consisting of explanatory variables is created as a node, and a model is automatically created to derive prediction results at the "leaf" part.
The advantage is that it is possible to clearly visualize what is being determined as a feature. In addition, it does not require pre-processing such as scaling, and can handle data of various scales as it is.
The disadvantages are that it is prone to over-learning and that it is not suitable for linear data.
A decision tree is a generic term for a model that combines a classification model called a classification tree and a regression model called a regression tree. . If what you want to do is classification, use a classification tree, if what you want to do is numerical prediction, use a regression tree .
The learning steps include the following flow.  
 - collect all the training data in the root node to build the tree.
 - build a tree with a single explanatory variable such that the data with teacher labels is optimally partitioned under a single explanatory variable The source data is divided by selecting one explanatory variable and setting the threshold value in that variable.
 - divide the data again at each node.
 - repeat steps 2 and 3 at each node until the final optimal division is achieved.

2. Explain the meaning of clustering and state its difference with classification.  
Clustering is a method of finding collections in the data.
Classification is a method where the teacher data is used to show the computer how to divide the data in advance. Although necessary, clustering finds gatherings in unsupervised learning from the data.

3. Describe the k-means clustering algorithm, in no less than 200 English words.  
The k-means method is an algorithm which divides the data into appropriate clusters and adjusts the data by using the average of the clusters to divide the data nicely.
It is called the k-means method because it is an algorithm to create k clusters of arbitrary size, and therefore it is called the k-means method.
The k-means method follows the following process
```
 - randomly assign a cluster to each point x.
 - calculate the center of gravity for the points assigned to each cluster.
 - calculate the distance from the center of gravity calculated above for each point, and put the distance to the nearest cluster Reassign the cluster.
 - do steps 2 and 3 until the cluster to be assigned no longer changes.  
```
The problem with the k-means method is that the accuracy of the k-means method varies depending on the initial random cluster assignment.
An algorithm that solves this problem is k-means++. k-means is an algorithm that uses randomly determines the center of gravity, but k-means++ randomly determines the center of gravity at one of the first data points Pick one and make it cluster-centric.

# week10 -Analysis of Information(3)-
1. Explain what the agglomerative clustering and the divisive clustering are, respectively.  
Divisive clustering is the process of dividing individual data points into separate classes It is a method of clustering that starts as and merges the two most similar clusters. Respectively clustering means that splitting clustering is a technique in which the algorithm to divide the cluster into sub-clusters until the specified stopping point is reached. It is a method of cluster analysis that is performed repeatedly.

2. Describe the basic Hierarchical Agglomerative Clustering (HAC) algorithm, in no less than 200 English words.  
Agglomerative hierarchical clustering is a simple iterative classification method in principle.
```
- The process starts with the computation of dissimilarity between the N objects.
- When two objects minimize an arbitrary agglomeration criterion, they are in the same cluster collected and thus the two objects constitute a single cluster.
- The dissimilarity between this cluster and N-2 other objects, using the agglomeration criterion Calculation. Then, the clustering of two objects or objects that minimize the agglomeration criterion by clustering The clusters are assembled in the same cluster.
```
This process continues until all the objects are clustered.
This process is generally represented by a tree diagram. The process of clustering proceeds from the bottom of the tree tree to the top.
Fusion between clusters occurs at the point where the two lines intersect. The height of the point of intersection represents the order of the fusion, the lower the height, the earlier the fusion has occurred .
If we cut this tree at a certain height, we get a set of clusters.  

3. State the major methods of calculating closest pairs of clusters in hierarchical clustering.  
The proximity between two objects is determined by the degree of proximity between the two objects and at what point they are similar or similar Since the HAC algorithm uses dissimilarity, it is measured by measuring If the user chooses a similarity, XLSTAT transforms it into a dissimilarity. The transformation for each pair of objects is to calculate the similarity of the pairs in question from the maximum similarity in all pairs Subtraction is done by subtracting.

4. Explain the way of using “purity” for clustering quality measurement, with an illustrative example.  
Purity means that in each cluster, the correct answer cluster belonging to the most included cluster It is a weighted average of the percentage of the number of elements. For example, a purity of 0.99 is a high quality product, while a purity of 0.30 is a high quality product. If we have a purity of 0.30, we can say that the quality of clustering is low.

# week11 -Analysis of Information(practice)-
[Question 4]
Answer the following questions regarding association rule mining.

In association rule mining, “support” and “confidence” are used for measuring the rule strength. Explain what “support” and “confidence” are, with illustrative examples. 
Describe the Apriori algorithm for association rule mining, in no less than 200 English words.

[Answer 4]
1.

Support is the percentage of occurrences of the rule "When you buy product A, you buy product B as well" in the total data. The higher this indicator is, the higher the percentage of occurrences of that rule (the combination of buying product A and buying product B) in the whole data.

Confidence is the ratio of the occurrence of conditional (A) and conclusion (B) at the same time in the ratio of the occurrence of conditional (A) items in the conditional part (A). The higher this indicator is, the higher the percentage of "When you buy product A, you also buy product B", so the two products (items), A and B, are strongly related. For this reason, it can be said to be an indicator with a meaning similar to the correlation coefficient.

 

 

2.

The Apriori algorithm is defined as the set of elements that are included in the data set to be processed over a certain number (given as a threshold minsup). Detecting the frequent item set is a fundamental problem in data mining and is a prerequisite for various applications, including correlation rule detection.

 

The algorithm for the detection of frequent item sets is illustrated in the following figure. As a process, a candidate set consisting of one element is first generated (C1), and then the frequent item set is "sieved" on the condition that the number of occurrences is more than a threshold, and the frequent item set is generated (L1). Next, the elements of the frequent item set (L1) are combined to form a candidate set consisting of two elements (C2), and the frequent item set is generated by "sieving" the candidate set on the condition that the number of occurrences is higher than the threshold value (L2). This process is repeated.
