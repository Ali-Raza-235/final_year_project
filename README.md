# Final Year Project

## Web Page Ranking System
## Project Domain / Category
<b> Information Retrieval(Python)/Software Application </b>

## Abstract / Introduction
        The aim of this project is to develop an information retrieval system that calculate the term frequencies, document frequencies and return the user, the top most ranked web pages in response to a query. The main advantage of this system is to help to reduce the efforts required to search a most relevant documents according to the query parameters.

        It will provide the most relevant documents according to his/her query from the bulk of documents that are available on the world wide web and saves the time and search effort of a user and leads to the most relevant documents within few minutes. 

## Functional Requirements:

       Provide a bulleted list of functional requirements
### 1. Preprocessing of provided data set
a.	In preprocessing, cleaning of data set is the key process.
b.	Detect the stop-words and punctuation marks and  remove both of these. 
c.	Convert the whole data in same case(i.e. lower case)

### 2. Read the file “Sample_dataset.txt”  and find total occurrences of word
a.	Write a function that returns count of number of lines in txt file. 
b.	Write a function that returns count of number of words in txt file. 

### 3. Write a function that returns a data frame with two columns having stop words in one col and their count in the other.

### 4. Now generate a .txt file named “Rollnumber.txt”(write your own Student ID) having all content of the given file but excluding stop words.

### 5. Write a function that prints the count of lowercase words in the file.

### 6. Perform lemmatization on the given file and generate a txt file named “Rollnumber_lemmatized.txt” having all content of the given file.

### 7. Perform stemming on the given file and generate a txt file named “Rollnumber_stemming.txt” having all content of the given file.




### 8. Read all .txt extension files(dataset.txt) and perform the following tasks: 
	Write a function named wordList(doc) in such a way that it takes a txt file as input argument and returns a list of words in your document. For example, for below paragraph 
Association for Computational Linguistics 6 th Applied Natural 
Language Processing Conference Proceedingsnof the Conference 
April 29--May 4, 2000 Seattle, Washington, USA ANLP 2000- 
PREFACE 131 papers were submitted 
It will return list of words like this 
['Association', 'for', 'Computational', 'Linguistics', '6', 'th', 
'Applied', 'Natural', 'Language', 'Processing', 'Conference',
'Proceedingsof', 'the', 'Conference', 'April', '29-- May', '4,', '2000', 
'Seattle,', 'Washington,', 'USA', 'ANLP', '2000-PREFACE', '131', 
'papers', 'were', 'submitted', ]

### 9. Write a function named removePuncs(wordList) that takes list of words then iterate through this list.   During iteration it do some processing on each word. Function should replace punctuation marks as well as \n. and check either this word in stop-word on not? if it is in stop-word then we didn't append this into resulting List. You must also handle case insensitivity of words. Output for above list should be like this. 
['association', 'computational', 'linguistics', '6', 'th','applied', 
'natural', 
'language', 
'processing', 
'conference', 
'proceedingsof', 'conference', 'april', '29may', '4', '2000', 
'seattle', 'washington', 'usa', 'anlp', '2000preface', '131', 
'papers', 'submitted']

### 10. Write a function named termFrequencyInDoc(wordList) which should take a list of words asinput argument, and output a dictionary of words such that each word that appears in the document is key in the dictionary and it's value is term frequency.

### 11. Write a function named wordDocFrequency(dicList) that takes list of dictionary as input argument, each dictionary in this list is the word that appears in the given document as keys and the no. of times the word appears as value. This function should construct a dictionary which has all the words that appear in the corpus as keys and no. of docs that contain this word as value.

### 12. Construct a function named inverseDocFrequency(dicList,base) that takes dictionary returned from wordDocFrequency functions above and outputs inverse document frequency of each word.

### 13.  This function named tfidf(docList) takes list of documents it calls the function wordList to split the document in list of words and remove stopwords and punctuation marks from them, then calls termFrequencyInDoc() uses its output to create dictionary of vocabulary using the function wordDocFrequency(), it then should call inverseDocFre() function. It then outputs a list of dictionary, where each document corresponds to the dictionary, its words should be keys values should be tf-idf score.

### 14. Write a code for VSM(Vector Space Model that returns the top ranked pages/links available on internet) and run the following queries, you must show the top 5 documents ranked according to the score. Function name should be like this vectorSpaceModel(query)

## Author

### Ali Raza
