# The Politics of Warehousing in the Inland Empire, CA: How did we get here?
## Poli 179 Final Project 
### By: Alyson Otañez

## Background
The Inland Empire (IE) is located in Southern California, east of Los Angeles, made up of the San Bernardino and Riverside counties. It has seen rapid economic and industrial growth as a result of the increased demand in e-commerce and fast delivery, which has led to decreased air quality, loss of green space, and health impacts to the region. Warehouse development and placement is an environmental injustice issue; over 300,000 individuals live within ¼ mile of a warehouse, ~60% are Hispanic or Latino. San Bernardino and Riverside are the top 2 counties in the United States, where over a third of their year is met with high concentrations of ozone.

The approval of new warehouses is decided at the local level. My research focuses on Ontario, Fontana, Rialto, Chino, and the March Joint Powers Authority who are the regions with the highest concentration of warehouses in the IE. My project seeks to understand conversations occurring at the local level, as if this a relatively understudied issue, with little understanding of its causes and effects. To understand the dynamic between warehousing and local governments, I chose to analyze the city council agenda/meeting minutes of the cities of interest. 

## Research Question
My main goal is to understand the dynamics between local governments and warehousing. I want to determine if there is a difference between conversations surrounding beneficial programs such as public recreation and transportation compared to warehousing. Is one type of program mentioned more?

## Data
Scraped the city council meeting agenda/minutes of Ontario, Fontana, Rialto, Chino, and the March Joint Powers Authority. Templates to scrape the data can be found in the `Web Scraping` folder. Each website was scraped indivually and combined into one file. A PDF (that must be downloaded to access the links) can be found in the `Data` folder, within the folder there is a small sample of the data for reference. 

Google Drive of combine data: https://drive.google.com/file/d/1or3ZNrS9mVwjXdhX2DUCPjRyUwgrauiv/view?usp=sharing 

**N = 5,526** 

## Methods
Latent Dirichlet Allocation (LDA): a topic modeling technique to extract topics from a given corpus as a set of probability distributions of word frequency within a topic, and topic size in a corpus.

1. Apply LDA model to the entire corpus to gain insight of overall topics in corpus (`LDA_Corpus.ipynb`)
2. Apply LDA model on a filtered corpus based on classified text on a set of keywords (`LDA_Keywords.ipynb`). Resulted in 3 different models based on: industrial, recreation, and transportation keywords. Compared the topic difference against the industrial model. 
3. Apply LDA model on a filtered corpus based on a given decade (`LDA_Decades.ipynb`). Resulted in 2 different models based on: 2003-2013 and 2014-2014 data. Compared the topic difference in these two models to establish changes over time. 

## References

### Background
Munoz Amparao, Phillips Susan, Ann Ruiz Mary.  
A REGION IN CRISIS: The Rationale for a Public Health State of Emergency in the Inland Empire, https://calmatters.org/wp-content/uploads/2022/06/State-of-Emergency-Public-Health-Request.pdf 

Most Polluted Places to Live. https://www.lung.org/research/sota/key-findings/most-polluted-places 

Which Inland Empire cities have the most warehouses? 
https://www.pressenterprise.com/2022/12/19/which-inland-empire-cities-have-the-most-warehouses/#:~:text=McCarthy%20said%20the%20map%20also,rounding%20out%20the%20top%20five. 

Kozlowski, A. C., Taddy, M., & Evans, J. A. (2019). 
The Geometry of Culture: Analyzing the Meanings of Class through Word Embeddings. American Sociological Review, 84(5), 905-949. https://doi.org/10.1177/0003122419877135

### Code
Jacob Murel. Train an LDA topic model for text analysis in Python. https://developer.ibm.com/tutorials/awb-lda-topic-modeling-text-analysis-python/ 

How to Compare LDA Models. https://radimrehurek.com/gensim/auto_examples/howtos/run_compare_lda.html#:~:text=You%20can%20do%20this%20by%20constructing%20a%20matrix%20with%20the%20difference.&text=Looking%20at%20this%20matrix%2C%20you,the%20topics'%20intersection%20and%20difference.

