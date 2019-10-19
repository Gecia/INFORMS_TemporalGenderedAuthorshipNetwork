

*** NOTE ***  


If you use this dataset in another publication, please cite the following publication:  

Bravo-Hermsdorff et al. "Gender and collaboration patterns in a temporal scientific authorship network" Applied Network Science (2019)  
DOI: 10.1007/s41109-019-0214-4  




*** DATA DESCRIPTION ***  


These data contain the nodes and edges of a bipartite authorship network constructed from publications in 16 peer-reviewed journals affiliated with the INFORMS society from 1952 to 2016.  Publication records were acquired using INFORMS PubsOnline (in the form of BibTeX entries) and the CrossRef REST API.  

Nodes are one of two types: author or publication.  Edges denote an authorship of a publication.  
Metadata includes:  
 - For the author nodes: gender label (female, male, or unknown).  Gender was first coded by an external API (genderize.io) and then refined by manual inspection.  
 - For the publication nodes: publication year.  
 - For the edges: author position as given by the order on the publication.  

See the associated publication (DOI: 10.1007/s41109-019-0214-4) for details on the collection process and a description of the data.  


Three files are provided:  

Author nodes file (AuthorNodes.csv):  
Each row denotes an author.  
Author_Node_ID - Unique author ID  
Gender_Label_Refined - Gender labeled used in the publication associated with these data  
Gender_Label_API - Author gender as outputted by genderize.io  
API_Confidence - Author gender probability as outputted by genderize.io  

Publication nodes file (PublicationNodes.csv):  
Each row denotes a publication.  
Publication_Node_ID - Unique publication ID  
Year - Year of publication  

Edges file (Edges.csv):  
Each row denotes an edge.  
Author_Node_ID - Unique author ID  
Publication_Node_ID - Unique publication ID  
Author_Position - Position of this author for this publication  

