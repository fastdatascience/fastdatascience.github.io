---
layout: post
title:  "Natural Language Processing"
date:   2023-03-11 00:05:28 +0000
categories: natural language processing
---

[Natural Language processing](https://fastdatascience.com/portfolio/natural-language-processing/) is everything to do with getting computers to understand human language. It's a branch of AI but is really a mixture of disciplines such as linguistics, computer science, and engineering.

Has your boss ever asked you to make a summary in Excel of how much all your customers spend? If the data is in an Excel already, then the task is easy.

But what if your company processes fixes to new-build houses. Every homeowner sends in a form with the problems (electrical fault, damp, damaged plasterboard) described in plain text. Your boss asks you to find the commonest construction faults. These are all in PDF files submitted by homeowners. How could you do this in Excel? Where would you even start?

![homeowner](/assets/homeowner.gif)

You might be tempted to read through a sample of the documents and summarise them qualitatively for your boss. Of course, this is not a bad idea, and will give you insights. But we can do more...

# Natural Language Processing

Unfortunately we don't yet have a tool as simple as Excel for analysing unstructured text data. But there is a whole field of study dedicated to this kind of problem: Natural language processing (NLP).

Computers are very good at calculating faster than we can - for example, averaging numbers to find the mean customer spend. But they are not so good at unstructured data, although they are getting better.

If I was tasked with synthesising faults from homeowner documents like in my above example, I would proceed as follows:

* get hold of the data in PDF or Word format and convert it all to plain text
* read through the text manually and identify any common patterns
* understand how this set of documents is a problem for the business and what result from an NLP exercise could save them money
* depending on the business analysis, potentially run the text data through an algorithm such as [LDA](https://en.wikipedia.org/wiki/Latent_Dirichlet_allocation), which could identify clusters (topics) in the document.
* if necessary, hand-label some examples and train a classifier which can categorise a new incoming document into electrical, damp, structural, scratch, etc (whichever categories we decide on)
* the business may want a deployed classifier which can triage incoming documents, or assign them to high or low risk, cost, complexity, or identify other information in the documents which help business processes.

![inspection report](/assets/inspection-report.gif)

# Why is NLP important?

Natural language processing helps us convert unstructured data sources, such as an unorganised set of documents, into structured values that a computer can process. Human language is very complex and hard to model. For example, linguists have debated for years which category human languages fall into in the [Chomsky Hierarchy of Languages](https://en.wikipedia.org/wiki/Chomsky_hierarchy).

When I first started in the field in 2007 (studying a [Masters](https://freelancedatascientist.net/freelance-data-scientist-cv/)), there was a lot of focus in NLP on developing sets of rules to model a language such as English. This is incredibly difficult and NLP systems would often break down when they encountered unfamiliar inputs (such as a strange sentence structure, slang, spelling and grammar mistakes, or unseen languages and vocabulary). Now, the field has moved towards more data-driven approaches, where tech giants such as Google can train large language models (LLMs) on terabytes of data, without needing a linguist to laboriously hand-code a language's grammar into a programming language. But the problem remains, that unstructured data is difficult to handle. Organisations with large amounts of documents are often sitting on an untapped goldmine because they do not have the expertise in-house to extract value from their text data. In any industry with large amounts of documents, such as legal, pharma, insurance, construction, regulation, R&D, or humanities research, a company which can leverage its in-house text data will naturally get a head start on its competitors.

# How is NLP used in business?

| Business function 	| Application of NLP                                                                                                                                                                                                                            	|
|-------------------	|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------	|
| Customer service  	| Chatbots on company websites. These reduce call centre costs and allow companies to run analytics on chat logs.                                                                                                                               	|
| Customer service  	| Triaging incoming emails using a classifier                                                                                                                                                                                                   	|
| Operations        	| Estimate the risk of a [clinical trial protocol](https://clinicaltrialrisk.org/) failing, or the cost of a repair.                                                                                                                            	|
| Operations        	| Machine translation: Google, Azure translate                                                                                                                                                                                                  	|
| Market research   	| Machine learning models such as Whisper can transcribe interviews with Key Opinion Leaders (KOLs) in pharma                                                                                                                                   	|
| Operations        	| Document summarisation models                                                                                                                                                                                                                 	|
| Operations        	| Identify key products or locations mentioned in a text, and extract their relationships. For example, a doctor says "I would prescribe (DRUG) with (DRUG)", and a smart model may be able to identify the relationships between the entities. 	|


# How does NLP work?

There are two main approaches to NLP: symbolic NLP and statistical NLP, although a hybrid is becoming more popular.

* Symbolic NLP was the dominant approach from the 1950s to the 1990s, and involved programmers coding grammar rules and ontologies into a system, cataloguing real-world and linguistic knowledge.
* Statistical NLP is currently the dominant approahc, where machine learning algorithms such as neural networks are trained on vast corpora of data, and learn common patterns without being taught the grammar of a language.

# How can I learn NLP?

There are some excellent books and videos which I would recommend:

## Speech and Language Processing by Jurafsky and Martin

![Jurafsky and Martin](/assets/jurafsky_martin.jpg)

*Speech and Language Processing* was my core textbook when I studied my Masters in NLP in 2008 and is still top of the list. *Speech and Language Processing* is a general overview of traditional and modern approaches in the field, encompassing the two subfields of text and speech which are sometimes dealt with separately. Daniel Jurafsky and James H. Martin have kept their book up-to-date with new developments in the field, such as word vector representations. The book has a strong applied focus that allows users to apply their skills in real-world situations, and the authors have put the third edition draft [online](https://web.stanford.edu/~jurafsky/slp3/).

## Foundations of Statistical Natural Language Processing by Manning and Schütze

This book is also available [online](https://nlp.stanford.edu/fsnlp/promo/) and presents a thorough introduction to statistical approaches to natural language processing.

## Natural Language Processing with Python: Analyzing Text with the Natural Language Toolkit by Bird et al

If your language of choice is Python, this book will help you get off the ground quickly using a valuable Swiss army knife, the [Natural Language Toolkit (NLTK)](https://www.nltk.org/).

## Deep Learning by Goodfellow, Bengio et al

The [Deep Learning Textbook](https://www.deeplearningbook.org/) is a great comprehensive guide to everything related to machine learning and neural networks. It will help you understand the theory, whereas the NLTK book above is about practice.

## Video series: Hugo Larochelle

Hugo Larochelle from the Université de Montréal has put an [excellent series of video lectures online](https://www.youtube.com/watch?v=ciNBQupWsAc).


# Getting started with Natural Language Processing

If you have a large number of unstructured documents and you are struggling to extract value from them, please get in touch with us at [fastdatascience.com](https://fastdatascience.com/contact-2/).
