# prj_romance_three_kingdoms
## Introduction
Romance of the Three Kingdoms, written by Luo Guanzhong, is famous as one of the four greatest Chinese novels, which is devoted to the turbulent years in the end of the Han dynasty and the Three Kingdoms period in Chinese history. This book was created on the basis of the historical text Records of the Three Kingdom. Many researches have been done for these two great works.

However, traditional literary research methods rely on intensive reading of texts, which requires much effort for analyzing a novel with more than 1000 characters. Besides, such a qualitative method based on subjective feeling leads to the lack of objectivity.  

With the rise of computational linguistics, social network analysis which uses computer tools to analyze text characteristics has become an important approach to literary research. In a social network, the characters of a novel are regarded as nodes, and the relationships between them are described as edges. With the help of the great computing power of computers, the complex relationship between characters in a novel with thousands of words can be clearly presented through visual diagrams. And a lot of hidden information can be mined more easily. In addition, the quantitative methods such as calculating node centralities can be applied to analyze the importance of main characters, which makes the research results more objective and convincing.   

This project primarily aims to reveal the social network structure of the Chinese novel Romance of the Three Kingdoms to verify existing literary theories. 
## Literature review
Social network analysis uses quantitative methods to study the relationships between nodes in a social network, and visualizes these relationships through computer tools. Many scholars and researchers have explored the ways to apply social network analysis to the field of literary studies. 

The research of Alberich, Miro-Julia and Rossello (2002) showed that the social network in Marvel Comics is very similar to the networks in real world. 

Stiller and Hudson (2005) revealed that the relationship networks of characters in the ten plays of Shakespeare are in line with the “small-world” model. 

Elson, McKeown and Dames (2010) analyzed the social networks of 60 English literary works in nineteenth century. The networks were extracted by looking at the quotation marks which indicate dialogues. The techniques of natural language processing and machine learning were used to determine all possible names of each character and the characters involved in each dialogue. This research studied the properties of each social network, and showed that there are significant regional differences in social interactions in nineteenth century English novels. 

Agarwal, Kotalwar and Rambow (2013) explored the technology for accurately extracting social events and social networks from novels. They used their corpus to train support vector machines, and put this method into practice by constructing the social network in the fiction Alice in Wonderland. 
It is worth pointing out that Stanford University established the Literary Laboratory in 2010, aiming to use computer tools to analyze literary works. Researchers used social network analysis and graph theory to study the plots in the play "Hamlet" and the series of novels "Harry Potter", and conducted empirical researches for existing theories. 

The researches mentioned above show that it is completely feasible to apply the approach of social network analysis to studying the structure and relationship between characters in a literary work.
## Methods
The procedure of this project can be divided into collecting data, preprocessing data, constructing social networks and analyzing social networks.

The data for this project are the English translation of Romance of the Three Kingdoms by C. H. Brewitt-Taylor. They are obtained by web sraping.

Before constructing the social networks, the plain texts should be preprocessed by natural language processing technology. The first step will be tokenization, which splits the sentences into single words. Then the names of each character will be extracted, using named entity recognition. 

With such a dataset containing words and names of characters, we can start building the social networks. In social networks, people are usually viewed as nodes, and their interconnections are viewed as edges. In this project, the edges will be determined by the co-occurrences of two characters in the same paragraph. And the weights of each edge will be determined by the frequency of co-occurrences. Thus, by counting the frequency of co-occurrences of two characters, we will construct weighted undirected social networks.

After the social networks are built, statistical analyses will be performed. For example, protagonists and the most influential people will be detected by node centralities. Also, interest groups can be revealed by the algorithm of community detection. In addition, the development of the plots in the novel can be demonstrated by the change of social networks in different chapters.

The steps mentioned above will be realized with the help of Python, Gephi and other additional computer tools. 
## Expected results
At the end of this project, social networks in the novel Romance of the Three Kingdoms will be constructed. Analyses of the social net works will be conducted to reveal the most important characters as well as the structure of this novel. Finally, comparative research will be done with with extracted network.
