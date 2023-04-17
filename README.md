# SNA Final Project: Pixar Easter Eggs
This repository is for our Social Network Analysis project, Pixar Easter Eggs. Completed by Indigo Parlin, Sophie Varma, and Annie MacIntosh in April 2023. 

## Contents

1. [Google Colab Notebook](https://github.com/indigoparlin/sna-pixar-easter-eggs/blob/main/pixareastereggs.ipynb)
2. [Easter Eggs Data](https://github.com/indigoparlin/sna-pixar-easter-eggs/blob/main/eastereggs.csv)
3. Google Slides
4. [List of Data Sources](https://github.com/indigoparlin/sna-pixar-easter-eggs/blob/main/sources.txt)


## Question
How is the Pixar Cinematic Universe Connected? 

## Introduction
We all know about the Pixar Easter eggs. It’s impossible to watch a Pixar movie without catching a glimpse of Pizza Planet. But how connected are the 27 Pixar movies, really? Our project sought to find out how many connections exist between each movie and which movies were most important in facilitating the network structure of Pixar movies. 

## Research Method
In order to create our initial dataset, we researched easter eggs from each Disney Pixar movie, looking at Toy Story (1995) up until the recently released Elemental (2023). Using information from blog posts and videos from Disney blogs and fan websites ([see full list of sites here](https://github.com/indigoparlin/sna-pixar-easter-eggs/blob/main/sources.txt)), we created a matrix in Google sheets that connected emblems of Pixar in the film they appeared in to the film they were originally from. We also documented the appearances of the Luxo (Pixar) Ball and the Pizza Planet Truck which are two symbols that supposedly appear in every Disney Pixar movie, starting with Toy Story. 
We utilized Python Package Networkx to compute our results in a Google Colab Notebook. You can view our [eastereggs.csv](https://github.com/indigoparlin/sna-pixar-easter-eggs/blob/main/eastereggs.csv) and [pixareastereggs.ipynb](https://github.com/indigoparlin/sna-pixar-easter-eggs/blob/main/pixareastereggs.ipynb) in this repository. 
