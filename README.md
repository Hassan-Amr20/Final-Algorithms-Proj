# Final-Algorithms-Proj
Team Members:
Hassan Amr 202400377	
Mohamed Elhalawani	202403388
Belal sherif	202401318
George Mina	202402179
Mazen Fouad 	202402454
Khairy tarek	202401089
Karim Sabbagh	202400206
Mohamed Ayman	202201208
Judy shehabeldin	202401418

Contribution Statement:
1. Project Overview & Problem Statement Mohamed Halawani
2. Dataset Category Selection George
3. Dataset Processing & Graph Construction Mazen
4. Dijkstra Algorithm Belal
5. Bidirectional Dijkstra Khairy
6. ALT Algorithm Belal
7. MultiLevel Dijkstra Mohamed Ayman
8. PLL Algorithm Belal
9. Snapshot Generation Hassan
10. GraphML Export & Visualization Pipeline Karim
11. Video Generation Judy
12. Experimental Results & Runtime Analysis Hassan
13. Conclusions, GitHub, and Project Management Hassan
14. Presentation Slides Mohamed Halawani
    
The idea behind the project is to see how different SSSP algorithms perform differently for different size treess and to visualize how these algorithms iterate through the trees.

The Economic Trade Network Datasets Used:
- econ-wm1
- econ-poli
- econ-mbeacxc
- econ-orani678
- econ-psmigr1

The Algorithms Tested:
- Dijkstra
- Bidirectional Dijkstra
- ALT
- MultiLevel Dijkstra
- PLL

AI use decleration:
Since the idea behind the project is to analyse how the algorithms build trees and visualize and also due to our lack of prior knowledge about the different algorithm types, we had some amount of AI assistance while implementing parts 4-8.

The Methodology is as follows: we load all 5 datasets of different sizes from networkreposiory.com, afterwards we run each dataset through our 5 algorithms. As each algorithm runs snapshots are taken at certain intervals to obtain 20 snapshots of the tree as it grows. We also kept track of runtime for each. The runtimes for each dataset/algorith combo were saved in a table and graphed to visualize the complexity growth of each algorithm. The snapshots previously taken were then sliced together to make videos allowing us to see how the trees are formed by iteration.

The results of the runtime table, the colab notebook, the presentation slides, and the videos are attached in this repository.

Final Analysis:
We tried graphing runtime VS node counts and runtime VS edge count and decided edge counts provided a stromger correlation.
PLL was the fastest growing by far as our test datasets grew in size. ALT was also quite fast growing. Regular Djikstra and multilevel Djikstra performed very similarly, with both being better than PLL and ALT. Bidirectional was the best performer with small growth in runtime even with much larger tree size. From this analysis Bidirectional Djikstra is the best option for this type of tree(economic netwowrks).
