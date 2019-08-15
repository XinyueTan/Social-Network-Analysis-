# Social Network Analysis
![2de530740731a175c103748713f8fced](https://user-images.githubusercontent.com/46146748/63127038-62273800-bf7f-11e9-914f-bd1c431c76f2.png)

## Goal of the analysis

In this project, I will be working towards building three social network diagrams (graphs/sociograms) of a school classroom based on three different measures and then analyzing both centrality measures and clusters within the network. 

I use data from:

Representing Classroom Social Structure. Melbourne: Victoria Institute of
Secondary Education, M. Vickers and S. Chan, (1981)

Available from the Index of Complex Networks ([ICON](https://icon.colorado.edu/#!/))

The data were collected by Vickers & Chan from 29 seventh grade students in a school in Victoria, Australia. Students were asked to nominate their classmates on a number of relations including the following three "layers":  

1. Who do you get on with in the class?  
2. Who are your best friends in the class?  
3. Who would you prefer to work with?  

I will identify isolated students in class, given that there is an observed correlation between an individual connectivity to peers and their overall academic success. 

## Packages Required
```
install.packages("igraph")
```

## Procedures
1. Load three csv files ("best.friends.csv", "get.on.with.csv", "work.with.csv") as data frames
2. Manipulate each of the data sets so that it is suitable for building a social network using iGraph
3. Create a graph for each of the data sets. Visualize each of the graphs and color the nodes according to gender
4. Measure centrality (e.g.: degree centrality, closeness centrality, betweeness centrality)
5. Calculate the size of the largest clique(s),*nodes/vertices* in the largest cliques and the number of *maximal cliques* in each of the networks 
6. Find the *cutpoints (articulation points)* for each of the three networks

# Visualizations
Create a graph for each of the data sets. Visualize each of the graphs and color the nodes according to gender.

### Graph for "Best Friends" Dataset
<img src="https://user-images.githubusercontent.com/46146748/63126213-5fc3de80-bf7d-11e9-9aa5-cef86210e1f7.png" width="600">

### Graph for "Get On With" Dataset
<img src="https://user-images.githubusercontent.com/46146748/63126325-a1ed2000-bf7d-11e9-95a6-58e2d635d9be.png" width="600">


### Graph for "Work With" Dataset
<img src="https://user-images.githubusercontent.com/46146748/63126468-f5f80480-bf7d-11e9-9142-47ba6e784b60.png" width="600">

 
## Background
Social network anlaysis (SNA) has found utility is institutional, classroom and analyses of networked data in socially-based educational games. However, the utility of the method largely rests on being able to ascribe meaning to the **structure of the network**. Without meaningful interpretation of structure there is no added value to a networked model, teacher will find more suvccess simply regressing your outcome against student characteristics.  Understanding measures of centrality and network structure in SNA are therefore an important, though difficult, aspect of the method. As with all SNA work, the vocabulary can be daunting though the ideas are relatively intuitive.

Social network analysis (SNA) can be used to address research questions related to the level of participant engagement, identification of central participants and isolated students. Also, SNA provides instructors with the capacity to visualize group cohesion, network density, and evaluate the impact of intervention strategies on student engagement and connectivity by evaluating the evolution of participant relationships within discussions forums

## Definitions and concepts
* **Isolated students**: appear as nodes with no connections in terms of social and academic. Connections between nodes are weighted according to the number posts and replies made between the participants

   *E.g.: in the world of online learning, participant who has submitted a post but no other participants have responded can be indicated as an isolated user.
   *E.g.: in the world of online learning, attrition rates are frequently reported as higher than their on-campus counterparts. This has in part, been attributed to a lack of connectivity that is both social and academic, with fellow learners and the institution. Thus, any aids that can be afforded to forum facilitators to more accurately identify students that have not connected or have dis-engaged with the learning network early in their academic study, may assist with addressing concerns related to online attrition. 

* **Sub-groups or cliques**: may indicate strong bonding among a core set of students. However, the formation of these strong cliques can be to the detriment of other actors attempting to engage. The formation of these groups can also limit the diversity of engagement with peers. 

   *E.g.: in large class forums students will form cliques based on perceived academic potential. An effective strategy may include 1) assigning participants to new groups and establishing additional group specific discussion forums. 2) encourage participants to interact across multiple cliques (i.e. bridge structural holes) to foster intergroup idea sharing.
   
  
## Author
[Katherine Tan](www.linkedin.com/in/katherine-tan-2019), M.S student in Learning Analytics at Teachers College, Columbia University
