# Network-Analysis-Dissertation
StackOverflow, one of the world’s largest Community Question Answering platforms, has become a major IT source for programmers. 

However, in order to understand the changing trends of topics to users in StackOverflow, this project will build the network based on the

tags data from StackOverflow and find the central nodes of the network by comparing and calculating the parameters of multiple classical network models.

Dynamic analysis in this project will show the evolution of the network structure and community over time, reflecting the changing trends of users’ focus of IT topics.
# The first part is Data Collection
This Part finished at 8th June, Using API tool to collect question data from StackOverflow. The results show the 2022.1-2022.2 questions data(tags, view_count, score...). And make the tags as nodes, same questions include in different tags as edges.
This results saved as 'edges.csv'
