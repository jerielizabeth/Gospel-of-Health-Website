<!-- 
.. title: Project Overview
.. slug: overview
.. date: 2018-02-01
.. description: 
.. type: text
-->

[anecdote to start]

The United States in the nineteenth century was "awash in a sea of faith"... 

In this dissertation, I examine the unique religious culture that developed during the first eighty years of Seventh-day Adventism. I argue that cycles of end-times expectation and the religious leadership of Ellen White contributed to the formation of a religious culture marked by domestic authority, cooperative organization, and the activism of women, seen in the movement's religious understanding and pursuit of health. This culture provides an instructive counterpoint to accounts of nineteenth-century revivalism that stress the reinforcement of patriarchal structures and capitalistic economic structures in the aftermath of the revivals of the nineteenth century.


## Understanding Religious Revivals


- C.S-R / Douglas on disruption and power
- Geertz and culture as assemblage of texts
- Turner and liminality
- Hatch and individualism
- Anderson and Print

## Exploring Religious Literature Computationally

Seventh-day Adventism offers an opportunity to explore these patterns differently. Whereas revivals within the more established and often studied denominations, such as Methodist, Baptist, or Presbyterian, were marked by periods of disruption and reestablishment, in Seventh-day Adventism, we 
The religious sect developed out of 

Rather than focus on a particular period of heightened religious fervor across traditions, 

Methods that fit these theories

reading. 

distant reading through topic modeling 
engage this with theory

In the digital humanities, all of these approaches are often bundled under an umbrella of "distant reading," a phrase attributed to Franco Moretti, and used to convey the approach of looking across a range of texts for broader patterns.^[These can be patterns of language use (cite), patterns in genre and literary development (cite), ...] While the phrase has its own contested history, it is useful for conveying that these forms of computational processing enable the reader to "zoom out," to assume a different view point on a set of materials in order to identify new questions.^[Footnote about how this is contrary to a more objectivist understanding of how computational methods work and the type of knowledge they create. Cite Rhody; Klein.] By create a composite document of sorts, one that is always in conversation with the originating texts, scholars using these methods construct a useful representation which can ...

"All models are wrong; some models are useful." In offering an abstraction, all models of historical events, whether formed using computer algorithms or narrative structures, simplify the irreducible complexity of the past in order to offer an explanatory thread that helps us understand and respond to the past. Marxist theorists have helped illuminate the ways economic forces ... ; . At the same time, some models are more wrong and damaging than others. The "Lost Cause" narrative, ..., offers a model for understanding the American history that not only does not fit the evidence of the past, but has been used to reinforce racial and class structures that ... 

In applying computational models to the past, the historian is engaging multiple layers of interpretation 
we are applying particular interpretive models - understandings of how influence works within social networks, patterns of language use and reuse, how words carry meaning - to our interpretation of the past. This is both 

Some computational problems are relatively straightforward: text reuse is a particularly salient example, though complicated by questions of what the parameters are to qualify as "reuse."  
Examine patterns in Seventh-day Adventist responses to millennial anticipation ... such projects offer excellent material for focused studies of particular facets 

Computational analysis as the basis for more traditional heuristics such as reading and, for historians, contextualization, 

One ongoing challenge for humanities research that uses computational methods is that of "hermeneutics," of bridging the contributions of computational work to the processes of knowledge in the respective humanities fields, of connecting theory and method into knowledge.^[@Clement2016, ] 


Use the model to reveal a pattern and to trace its general contours. Could be done differently - could rely on selective reading to identify and argue for general contours (examples). Advantages of the computational model include 1. that it enables use of a large corpus; 2. is reproducible in ways that reading is not; 3. aids in finding unexpected patterns and correlations. The mathematical model can give us insight into that which we cannot "see," provide an abstraction that enables us to identify where to look. 

- problem of "objectivity"

### Reading Religious Culture through Topic Models

Topic modeling is an umbrella term for a variety of different algorithmic approaches to summarizing documents by identifying words that tend to appear together. While the mathematical details vary, these approaches take as inputs a collection of documents and a desired number of topics, and then use that information to assign the words in a document to the various topics, updating those assignments based on the probability of words occurring together across all of the documents.^[For more detailed descriptions of the overall contours of the approach, see Brett; Jockers; Rhody] The algorithms produce two primary outputs: a list of words and their prevalence in each topic, and a list of topics and their prevalence in a document.

Of the different approaches to topic modeling, latent Dirichlet allocation (LDA), first developed in 2003, has become widely used and widely extended.^[Cite Blei, @Boyd-Graber2017, 7] LDA provides a model of topics present in a document and the words present in a topic, according to the assumption that individual documents are about relatively few topics and that topics are, on the whole, composed of relatively few words. The LDA parameters result in models where words can belong to multiple topics, and where documents are composed of a small set of topics. This is a representation of one way language works in written documents. There are certain words that are frequently used together when one is writing about sports, or zoology, or theology. In addition, documents tend to be focused on a small number of subject areas. Blei and others used those features of writing and language use to capture those words that occur together in a text and use that collection as a description of documents and corpora. 

As researchers have applied LDA in multiple contexts and for a growing number of research questions, the algorithm has also been extended to model aspects such as authorial distinctiveness, change over time, and correlation between topics.^[cite ..] By adding parameters to emphasize relationships between elements into the algorithm, such as between topics, between authors and their works, and between time and word usage, these extensions of LDA can quickly and powerfully model a range of factors that shape the development of texts. Of these, a correlated topic model, which identifies topics that tend to occur together, and a multiple-corpus model, which enables the creation of an overall model while capturing the distinctiveness of the constituent document collections, are two approaches which would likely yield productive results in exploring the literature of the Seventh-day Adventist denomination. 

However, while these more specialized applications of LDA provide tools for exploring particular aspects of a corpus, my goal for this dissertation is to establish a baseline of sorts for using topic modeling in studying the development of religious movements. As the literary form produced by the early Seventh-day Adventists differs from the materials typically used to train topic modeling algorithms, and their cultural context is markedly different from that of the academic and encyclopedic literature typically used to develop and train the algorithms. This is not to claim that the the algorithms are not robust enough to accommodate those differences, just that it is useful to establish how the materials and the algorithm interact before applying algorithms that assume the contours of the very change I am setting out to explore.^[cite Schmidt]

Looking from the fast-paced world of natural language processing, where new methods are continually expanding the ways we can computationally explore text, it is perhaps jarring to turn back to topic modeling. While the method spurred a flurry of blog posts and digital humanities projects in the years around 2010, in the time since newer approaches, such as word embeddings, and different questions, such as text reuse, have dominated the scholarly landscape.^[Cite Schmidt, Heuser, Viral Texts, Mullen. Exception is Kaufman] These approaches are proving quite powerful, enabling scholars to explore focused questions around word use and language shifts with word embeddings to publication networks, information dissemination and the history of ideas. 

Topic modeling does, however, offer some significant advantages for the types of questions often pursued in historical research. Developed in response to problems of information retrieval, topic modeling is a form of distant reading focused on capturing the broad themes and overall contours of a large collection of documents. Significantly, it does not require human readers to categorize the documents or the define the themes ahead of the analysis. This has two advantages. First, it makes it possible to work on large collections of relatively unknown textual content. And second, it creates opportunities to capture "unexpected" themes and trends. Where a researcher who relies on manual categorization may have to process through the documents multiple times as new categories become apparent, topic modeling algorithms use word frequency information to capture the assigned number of topics, independent of which topics a researcher is interested in.

The degree of distance that topic modeling provides is also well suited for historical research. The algorithm focuses on word co-occurrences within documents, with "document" defined by the researcher. As a result, the "topics" offer document-level descriptive information, which provides an overview of the "types of things people talked about" in a given set of documents, while also pointing back to the original documents for further study on topics of interest. The "bag-of-words" representation used by topic modeling, where the algorithm considers the document to be a unordered collection of words and their counts, is both a strength and a weakness of the approach. Although this representation reduces the direct contextual information about word use, a loss that is costly for explorations of word meanings and associations, it is much less costly at the level of document description. When functioning as an index of sorts, the data from topic models directs researchers to documents of interest. At the same time, the model itself offers information about the general contours of the document collection, and when combined with the document metadata, can be used to indicate when and where particular topics were prevalent, and can be used to suggest related topics. 

### Interpreting the Models

While a powerful algorithm for summarizing large collections of documents and guiding research questions and further reading, topics models can be difficult to verify and interpret, making them an easier algorithm than many to "lie" with. The strength of the algorithm is that it can illuminate "latent," hidden, patterns or topics, but it is also possible for those topics to be noisy, to include words that don't fit or only fit due to coincidence. In addition, the algorithm will organize the words of the corpus into as many topics as the user designates, and the resulting model can appear "readable" at different numbers of topics.^[Schmidt discusses this "danger" of topic models in JDH.] As a result, while the resulting models are useful, it is important to remember that they are abstractions of patterns in word co-occurrences and, like all models, are wrong in certain aspects. 

In anticipation of some of the challenges of interpreting topic models , I have paid close attention to the creation of the model, including my work to select and preprocess the documents, and steps to verify the model. 


While digital humanities scholars have been experimenting with topic modeling for some time, there is not yet consensus around how to use these models in humanities scholarship. Surveying the literature, projects that use topic models can be grouped into three main categories: topic models for exploration and discovery; topic models for statistical relationships; and topic models for corpus description. 

Rely on reading - reading the words to assign topics; "reading" the graph to identify patterns; reading the originating texts to identify meaning.

I am proposing a third way between the Jocker's reliance on statistically significant relationship and the more descriptive uses of topic models. 

Leverage the mathematical model to identify two features: 1. when "end-times" topics spike and dip relative to the rolling average, and 2. which topics correlate with "end-times", and which spike after a period of "end-times" expectation. This proves a general overview of the corpus literature. 

I posit that early Seventh-day Adventists experiences cycles of end-times expectation, with these cycles increasing in length as one moves forward from 1844. I also posit that, although the focus on of the group shifts with time, adherents embraced a  

theoretically i am more interested in the variations, in the idiographic, than in the general or nomothethic. 



Can a knowledge claim be made based on showing a statistically significant relationship between features? Is persuasive prose, supported by broad and significant archival evidence and theoretical finesse, the mark of a good historical argument? To invoke Gertrude Stein, what is the "there" of historical scholarship and 


## A Note on Religion

As with other areas of history where there is an active community with a vested interest in the history told, it is common for scholars of religion to state their own religious history and affiliation. For the Seventh-day Adventist community, the literature about the denomination has, to date, tended to fall into two general categories: sympathetic histories by Seventh-day Adventist authors and critical histories by authors external to or critical of the faith.^[Note a few examples] This has led to some concerns when new faces appear asking questions, concerns politely expressed to me as I started visiting Seventh-day Adventists archives and research centers. My having read Ron Number's *Prophetess of Health* did not help my efforts to establish myself as a credible commentator.

At a recent conference of the Association for Seventh-day Adventist Historians, Nicholas Miller presented the following chart as a taxonomy of the varieties of religious histories.

[imbed chart]

My approach to the study of religion fits somewhere on the edges of the "Open Critical History." Along with many other historians of religion, I am interested in religious movements because I find religion and religious belief to be an irreducible category of analysis - something that shapes and explains the behavior of individuals and the development of groups, and that cannot be explained away through reference to economics or other social pressures. 

I came to the study of Seventh-day Adventism as an outsider - as someone raised in the small, historically Dutch, Christian Reformed denomination and brought up within the American "evangelical subculture." Seventh-day Adventism was not a religious group I was deeply aware of prior to beginning this study, and the process of learning to develop an understanding of a tradition far outside my own has been a transformational one. While I am sure that I have missed some of the details and nuances of the beliefs and structures I describe here, I have attempted to sketch the overall contours of the patterns I found and the ways those changed over my period of study. Any misrepresentations have been made unintentionally.






