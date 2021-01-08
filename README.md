

# Prediksi : A predictve text/markdown editor

#### Overview
Prediksi is a web app, hosted using django server. It provides general purpose online text/markdown editor with context aware word autocompletion.

#### Motivation
Most of the online and offline text/markdown text editors do not provide general english autocompletion and if they provide, those are not content aware i.e. autocompetions are not very much relevant.
 Prediksi tries to solve this problem by using users text to find the context/ topic of text and suggesting autocompletions according to the topic.
 for example in an article about 'Squirrel' initiating with squ we are most likely to type 'Squirrel' not 'square'.

#### Prerequisite
for analyzing the context this text edtor uses tfidf.
to calculate tfidf, document frequecy is used i.e. document frequency of a word is  number of documents in which that word is present., this document frequency is precalculated on 3600000 wikipedia articles and stored in a file named doc_freq_36lac.txt inside app/ folder. simmilar result can be produced by using app/doc_freq.ipynb file

#### uses
to set up your own text editor, 


1. ```git clone https://github.com/agusmakmun/django-markdown-editor```
2. ```git clone https://github.com/sandeshpatel/prediksi.git```
3. ```git clone https://github.com/MarioVilas/googlesearch.git```
4. ```mv prediksi/martor.js  django-markdown-editor/static/martor/js/martor.js```
5. ```pip install django-markdown-editor``` 
6. ```pip install googlesearch```
7. ```pip install numpy```
8. ```pip install django```
8. ```cd prediksi```
9. ```python manage.py runserver```

#### Demo Images

![](/Images/1.png)

![](/Images/2.png)
