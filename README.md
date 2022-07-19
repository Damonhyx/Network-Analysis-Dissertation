# Network-Analysis-Dissertation
StackOverflow, one of the world’s largest Community Question Answering platforms, has become a major IT source for programmers. 

However, in order to understand the changing trends of topics to users in StackOverflow, this project will build the network based on the

tags data from StackOverflow and find the central nodes of the network by comparing and calculating the parameters of multiple classical network models.

Dynamic analysis in this project will show the evolution of the network structure and community over time, reflecting the changing trends of users’ focus of IT topics.
# The first part is Data Collection
This Part finished at 8th June, Using API tool to collect question data from StackOverflow. The results show the 2022.1-2022.2 questions data(tags, view_count, score...). And make the tags as nodes, same questions include in different tags as edges.
This results saved as 'edges.csv'
I have deleted part of questions in the documents(scores lower than 5)

# 2-Network Analytics
Using the data in Barab´asi-Albert Model, Erd¨os-R´enyi Model, WattsStrogatz Model, and the Configuration Model. Calculating the Degree Distribution(for expamle BA): 
![BA Distr](https://user-images.githubusercontent.com/96798654/179717074-2b07bb51-6511-4e8c-9518-4fc2c8d24a9b.jpg)
And compared with real world network distribution:
<img width="985" alt="Real Distr" src="https://user-images.githubusercontent.com/96798654/179718494-c614f795-cfc7-4b26-a176-9de9eae72f66.png">


Connected Components, Path Analysis, Density Analysis and Clustering Coefficient(for example BA):
![BA Coffin](https://user-images.githubusercontent.com/96798654/179717953-f4b66eb6-354b-48a0-80cc-28e8ffb91cd8.jpg)
And compared with real world network distribution:
<img width="992" alt="Real Coffin" src="https://user-images.githubusercontent.com/96798654/179719724-00f0c08f-d683-493d-a4de-0061d1358314.png">

Comparation the degree and nodes in different model:
<img width="1012" alt="Compare degree" src="https://user-images.githubusercontent.com/96798654/179719532-5dc209f1-354a-4a9f-a7f6-37be27f8c31f.png">

And I used degree_centrality, eigenvector_centrality, pagerank_centrality, closeness_centrality, harmonic_centrality and betweenness_centrality to calculate the nodes' centrality coefficient to prove the central nodes in the networks.
![central 1](https://user-images.githubusercontent.com/96798654/179720422-4080760f-6ab4-4a8c-bedb-86a96dccd13a.png)
![central 2](https://user-images.githubusercontent.com/96798654/179720560-1175970b-7a61-4801-9e3a-63a04b183f89.png)


# 3-Community Discovery
I used the community detection methods and calculated the number of the communities from 2022.1 to 2022.6 respectively, finding the changing trend in community(especially the main nodes of every month). The community detection methods contains Girvan-Newman algorithm, Louvain, Label Propagation and Demon algorithm. And I calculated the numbers of communites and communities distribution in each method. Besides I finished calacuated the outcome of central nodes in every monthes.
