# Bring me the Horizon Bibliography - Documentation


<br>
<br>

## Corpus
The corpus included in this github repository is a corpus of song lyrics from the British Metalcore band Bring Me The Horizon. In the texts folder are 6 folders, corresponding to their six albums with commercial success, namely: ‘Suicide Season’, ‘There Is A hell Believe Me I’ve Seen It. There is a Heaven Let’s Keep It A Secret’, ‘Sempiternal’, ‘ That’s the Spirit’, ‘Amo’ and ‘Post Human: Survival Horror’. 
<br>
## Audice and use
The target audience for this project is people interested in lyrics analyses, programming, but also people who are fans of BMTH. This corpus can be used to have a handy CSV of the annotated lyrics of the six most commercially viable BMTH albums's songs, and can then also be used to analyze their music, style, word-use etc. The .txt of the lyrics itself and the columns containing these lyrics are deleted as the song texts are copyrighted. The tokenized and annotated columns are derivative versions of the text and are included for educational purposes.
## Text selection
This corpus only contains all albums released by Bring Me The Horizon from 2008 until now. BMTH has released an album before 2008, but it was not that popular. Besides this, the band has released many EP’s, singles and features, which were not included in the corpus. Only commercially viable albums have been chosen in this corpus, so that they can be compared.
<br>
## Data Collection
The lyrics have been manually copied to txt files from the website www.azlyrics.com, without altering the structure of the lyrics, except for deleting vocal attribution since it is not necessary for the uses of our dataset and inconsistent. Doing this I checked if the lyrics made sense, there were no mistakes and if there are redundancies. 
<br>
## Pre-processing
The bare lyrics are in txt files, one txt file per song. Furthermore, the txt files are spread over 6 folders, each folder corresponding to a album. These files have been converted to a CSV file using python. Using python, the CSV file has been cleaned, deleting newlines and transforming all text to lowercase.
<br>
## Annotations
To the original CSV I used the spaCy library to add Doc, Tokens, Lemma's, Part-Of-Speech and Named_Entities and their corresponding NE_Words to the songs. To make this easier I have converted the CSV into a dataframe. 
<br>
## Format
The song lyrics data has been annotated and explored in an IPython Notebook (ipynb file) called 'BMTH lyrics annotation'. The annotated lyrics themselves can be found in a CSV file called 'BMTH_Discography_annotation'.
<br>
## Description of columns in annotated CSV 
| Variable | Description |
| --- | ----------- |
| Album | The album this particular song belongs to |
| Song Name | The name of the BMTH song |
| Tokens | The tokenized text of the song lyrics |
| Lemmas | The lemmatized text of the song lyrics |
| POS | Part of speech of that the tokens in the song lyrics |
| Named_Entities | The categories of Named Entities that are in the song lyrics |
| NE_Words | The actual words of the Named Entities in the song lyrics |
| Total_Words_Per_Song | The total amount of words for every song in the corpus |
| Sentiment | The TextBlob sentiment score of every song lyrics in the corpus |
<br>
