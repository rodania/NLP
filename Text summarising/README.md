# Text summarising
## Target: 
Building model to automate text summarising
## The methodology
### 1. Obtaining Text
       Importing text that needs to be summarised. Online articles need further processing due to html structure. 
       Beautifulsoup4 library to parse html code.
### 2. Normalising text
       This includes: removing punctuation, using lower case, removing stop words, etc.
### 3. Building the histogram
       It's calculated by dividing the number of occurrences of each word by the number of occurrences of the word 
       which occurs most in the document. 
       It is assumed that the most frequent occuring words will be indication about the core subject of the text.
       Histogram is calculated on the cleaned text.
### 4. Calculating sentences scores
       Sentences will be scored using the word histogram calculated above. This is done by summing up the scores of 
       each word in a sentence and hanging on to the score. The maximum length of sentences is a parameter used to 
       prevent the summary would have only long sentences. Since long sentences are more likely will get the highest 
       scores than shorter ones. However, in the other side it can be considered a bias towards long sentences.
### 5. Finally, the summary
       The summary will have the top scored sentences

       
