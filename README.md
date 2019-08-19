TF-IDF model
Term Frequency
This measures the frequency of a word in a document. Word frequency is highly depending on the length of the document. 
For that reason, the frequency value is normalised by dividing the frequency by the total number of words in the document.

t — term (word)
d — document (set of words)
N — count of corpus
corpus — the total document set

                tf(t,d) = count of t in d / number of words in d

Document Frequency
measures how often the word appears in a document over how often it just appears everywhere
                df(t) = occurrence of t in documents

Inverse Document Frequency
                tf-idf(t, d) = tf(t, d) * log(N/(df + 1))
log is applied to scale values
and 1 is added to prvent dividing by 0

            

