.. title: Creating a Digital Dissertation
.. date: 2017-11-07
.. slug: about

.. contents:: Sections
   :depth: 2

My goal in constructing *A Gospel of Health and Salvation* as a "digital dissertation" has been to use the medium of a browser-based interface to bring together historical and computational analysis in a way that highlights the intellectual work involved in both. In my analysis, I have focused on the affordances of the presentation medium and the epistemological requirements of the different forms of analysis I have employed. In this process statement, I outline my rationale for the final structure of my dissertation and the technical components of the project. 

*********************************
Notes on Constructing the Project
*********************************

When I started working on the main part of the dissertation, my programming experience to date had been the two required digital history courses at George Mason University, an additional introduction to programming course, some hands-on experience in web development through my research assistantship at the `Roy Rosenzweig Center for History and New Media <https://rrchnm.org/>`_, and a `Rails Girls workshop <http://railsgirls.com/>`_. In retrospect, embarking on a technical project from that starting point was a bit over-ambitious. My initial design of the project included network analysis from the denominational Yearbooks and geospatial analysis of people, publications, and ideas, along with text analysis. While I still think that these additional modes of analysis would help illuminate the development of this particularly group of people, these ideas have been bracketed for future iterations of the project. 

Along the way, in seeking to solve different problems for the dissertation, I have learned enough programming to be dangerous (and to qualify for jobs as a junior web developer). I have also learned from the standards of practice in programming, data science, and library science for managing these new forms of content - datasets, code, and visualizations - in ways that are documented, readable, and reusable. Most significantly, however, is that process of learning to use different methods of computational analysis has made me increasingly aware of the fundamental epistemological questions involved in combining the divergent methods of meaning making in data science and history. This is the question that has become the underlying focus of the dissertation - how does one construct an argument using computational analysis that is both computationally sophisticated and historically meaningful? 

I used Python to complete most of the computational work in this dissertation, a choice informed by it being the language I gravitated toward in the introduction to programming course at George Mason and the usefulness of IPython Notebooks (now Jupyter Notebooks) for creating executable documents. In the time since I started on this project, R has become the default choice for computational work in the digital humanities, with its own solutions for reproducible work. While I would now recommend others start with R because of that strong community of practice, Python has the advantage of being a more generalized language, and has been particularly useful to me for the data preparation aspects of the project. [add sentence on D3 if I use it directly in redoing the browser interface.]

I have been overly determined in this project to do my own computational work, both because I am committed to the idea that one needs to grapple with the assumptions and implementation of both computational and historical analysis when bringing the two modes of inquiry together and because of the gender politics of the field. I am, however, deeply indebted to many people who have given their time and energy to help me understand and troubleshoot the technical aspects of this project. Chief among these are Fred Gibbs, the Experimental Humanities Group at the Iliff School of Theology, Lincoln Mullen, who consulted on the unfortunately tabled network analysis piece of the project, Amanda Regan, Taylor Arnold, and Lauren Tilton. The computational work in this project is primarily my own, aside from a myriad snippets gleaned from StackOverflow and the libraries and resources noted below. The one external contribution is the workflow for moving model files from DigitalOcean, where I ran Mallet due to the size of the corpus, to AmazonS3 for storage and locally for use, which was set up by Jason Wieringa.

Digital Sources
===============

As with any digital project, *A Gospel of Health and Salvation* is dependent upon digital sources upon which to operate. The digital sources were produced by the Seventh-day Adventist denomination. At the time of writing, these files are hosted at `the Online Archive <http://documents.adventistarchives.org/Periodicals/Forms/AllFolders.aspx>`_ of the denomination's Office of Archives, Statistics, and Research. The processes by which the periodicals have been digitized is not well documented. [More from email exchange with archivist.]


Computational Analysis and Digital Publishing
=============================================

Preprocessing done using Python and executed through a series of `Jupyter Notebooks <http://jupyter.org/>`_ for reproducibility. 

The final topic models were created using `Mallet <http://mallet.cs.umass.edu/>`_ through the command-line interface, while in earlier drafts I relied on `Gensim <https://radimrehurek.com/gensim/>`_.  

Analysis of the model done using Python, using the Pandas and Seaborn libraries for data analysis and visualization. [Final versions of the visualizations to be done in D3. I hope.]

I created the main dissertation website using `Nikola <https://getnikola.com/>`_, a Python static site generator. 

For displaying the model, I used Andrew Goldstone's `Topic Model Browser <https://github.com/agoldst/dfr-browser>`_, which relies on D3.js.

The documentation for my library of Python functions is generated by Sphinx from my inline code documentation and is hosted on ReadtheDocs.


***************************************************************
Archiving and Reconstructing *A Gospel of Health and Salvation*
***************************************************************

I have constructed the dissertation with an eye to the ways the project will be archived and for overall stability. The final outputs of the dissertation "text" are static HTML and data files, rather than a database-drive website with executable code. This format is easier to archive and requires less ongoing server maintenance to keep available on the web.  

[Archiving with the library]

Reproducing the Research
========================

The main components of the dissertation are split into four modules, two for computational processing, and two for presentation:

+ Python Library and documentation - https://github.com/jerielizabeth/GoH
+ Jupyter Notebooks - https://github.com/jerielizabeth/Gospel-of-Health-Notebooks
+ Website - https://github.com/jerielizabeth/Gospel-of-Health-Website
+ Model Browser - https://github.com/jerielizabeth/dfr-browser

Because of this structure, there is some duplication of files between the repositories. The moving of files is managed using the DoIt Automation tool.

[outline steps to reproduce the analysis]
