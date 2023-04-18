# SNA Final Project: Pixar Easter Eggs
This repository is for our Social Network Analysis project, Pixar Easter Eggs. Completed by Indigo Parlin, Sophie Varma, and Annie MacIntosh in April 2023. 

## Contents

1. [Google Colab Notebook](https://github.com/indigoparlin/sna-pixar-easter-eggs/blob/main/pixareastereggs.ipynb)
2. [Easter Eggs Data](https://github.com/indigoparlin/sna-pixar-easter-eggs/blob/main/eastereggs.csv)
3. [Google Slides](https://docs.google.com/presentation/d/1xjNP8PlhvaJi9nlzC-gwyqk15EAO6tIywFo-Z-hkzDY/edit?usp=sharing)
4. [List of Data Sources](https://github.com/indigoparlin/sna-pixar-easter-eggs/blob/main/sources.txt)


## Question
How is the Pixar Cinematic Universe Connected? 

## Introduction
We all know about the Pixar Easter eggs*. It’s impossible to watch a Pixar movie without catching a glimpse of Pizza Planet. But how connected are the 27 Pixar movies, really? Our project sought to find out how many connections exist between each movie and which movies were most important in facilitating the network structure of Pixar movies. 

*If you don't know about the Pixar Easter Eggs, here's an example: in "Monster's Inc," Boo holds a doll of Nemo, a character from another movie called "Finding Nemo."

## Research Method
In order to create our initial dataset, we researched easter eggs from each Disney Pixar movie, looking at Toy Story (1995) up until the upcoming unreleased Elemental (2023). Using information from blog posts and videos from Disney blogs and fan websites ([see full list of sites here](https://github.com/indigoparlin/sna-pixar-easter-eggs/blob/main/sources.txt)), we created a matrix in Google sheets that connected emblems of Pixar in the film they appeared in to the film they were originally from. We also documented the appearances of the Luxo (Pixar) Ball and the Pizza Planet Truck which are two symbols that supposedly appear in every Disney Pixar movie, starting with Toy Story. 
We utilized Python Package Networkx to compute our results in a Google Colab Notebook. You can view our [eastereggs.csv](https://github.com/indigoparlin/sna-pixar-easter-eggs/blob/main/eastereggs.csv) and [pixareastereggs.ipynb](https://github.com/indigoparlin/sna-pixar-easter-eggs/blob/main/pixareastereggs.ipynb) in this repository. 

## Results
![Graph produced by Networkx](https://github.com/indigoparlin/sna-pixar-easter-eggs/blob/main/graph.png)

**Movie most referenced by others:** Toy Story (1995)

**Least referenced movie:** Elemental (2023)

**Highest degree centrality:** Toy Story (1995)

**Lowest degree centrality:** Elemental (2023)

**Closeness centrality:** Toy Story (1995), followed by Monsters, Inc. (2001)

**Highest eigenvector centrality:** Toy Story (1995), followed by Monsters, Inc. (2001) and Finding Nemo (2003)

**Highest betweenness centrality:** Finding Nemo (2003), followed by Toy Story (1995)


**PageRank Results:**
The top three movies with the highest PageRank score are: Toy Story (1995), A Bug’s Life (1998), and Toy Story 2 (1999). 
The bottom three movies with the lowest PageRank score are: Turning Red (2022), Lightyear (2022), and Elemental (2023). 

The **histogram chart** represents the degree distribution of all the Pixar films by counting the occurrence of each degree. For example, the graph shows how 4 films have a degree of 18 (Finding Nemo, Toy Story 3, Inside Out, and Soul). The highest degree is 28, corresponding to Toy Story. This aligns with our earlier data in which Toy Story has repetitively had the most references to it from other films. In contrast, Elemental, which has not been released yet, has just one reference to it from another film. Nodes of degree 2, 3, 4, 14, and 21-26 are non-existent. 

![Annotated screenshot of histogram from Google Colab notebook.](https://github.com/indigoparlin/sna-pixar-easter-eggs/blob/main/degreehistogram.png)

## Analysis
Since Toy Story was the first film completed by Pixar, it introduced famous emblems of Pixar, including Pizza Planet and the Luxo Ball, which are present in all or nearly all Pixar movies. Thus, Toy Story is incredibly connected because all of these emblems connect back to this preliminary movie. However, it is important to note that although a number of movies point to Toy Story through different easter eggs, Toy Story does not point to any other Pixar Movie, as it was the first film by Pixar. 

This is a similar scenario to Elemental (2023), which is the newest Pixar film to be released later this year. Thus, Elemental does not reference to any other Pixar movie as its release date is in the future (June, 2023). However, one movie, Lightyear (2022) points to Elemental once. When Elemental is released, it is safe to assume that it will point to a number of other Pixar movies—most likely changing the data we currently have. 

The top three movies with the highest eigenvector centrality were Toy Story, Monsters, Inc., and Finding Nemo, respectively. This shows that these three films have the highest connections and references (pointing both in and out to other movies). This can tell us that these three movies may be the most influential Pixar movies—as they are the most interconnected. This makes sense as they are iconic to the franchise and some of the earliest films produced.

Pixar has a habit of creating teasers for their upcoming movie in each movie. Thus we can see a diagonal across the spreadsheet in the (x, x+1) diagonal.

Toy Story, A Bug’s Life, and Toy Story 2, all had the highest PageRank scores. These results are because they are three of the oldest films, thus they will almost always be referred to in later films. As opposed to the films with lowest scores (Turning Red, Lightyear, and Elemental), which are some of the most recent films to be created by Pixar—therefore there are not a lot of references to them in earlier films. 

Toy Story having the highest degree of 27  aligns with our earlier data in which Toy Story has repetitively had the most references to it from other films. In contrast, degrees 2, 3, 4, 14, and 21-26 are non-existent. The most popular degree is 18, with 4 films. One of these films is Finding Nemo, which is most likely referred to so many times because it is an all time classic (much like Toy Story). Therefore, it is often referenced by later films because it is so popular. In contrast, Soul and Inside Out are much newer films, which have a high degree because they reference many other older films. As they are newer films, they are able to reference more films than earlier films, such as Finding Nemo, simply because more exist to reference. This is the same reason why we have Toy Story and Elemental on opposite sides of the graph—the oldest and newest films which are referenced by almost all films or cannot be referenced by older films (respectively). 


## Impact & Future Research
Many people know about the Pixar hidden easter eggs but don’t know the depth that the animators go to include them nor the way that they connect Pixar as a Cinematic Universe. This project, for all movies up until Elemental (2023), provides a comprehensive network for film fanatics interested in seeing how their favorite films connect without having to track down the information in random Buzzfeed articles or re-watching all of the films themselves. As Pixar continues to create and produce more movies, the network we have created today will continue to expand. It will be interesting to continue this network analysis as new movies are produced, animators and production teams change, and as new iconic easter eggs and inside jokes, like A113, are created. 

