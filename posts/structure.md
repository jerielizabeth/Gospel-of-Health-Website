--- 
title: The Structure of A Gospel of Health and Salvation
slug: structure
date: 2018-02-01 00:00:00 UTC
description: 
type: text
suppress-bibliography: true
---

The culture of Seventh-day Adventism and the material realities of their historical records make the use of computational analysis both feasible and appropriate, while the question of time and gender required that I reflect back on the assumptions that shape the available computational algorithms. Communicating this bi-directional work posed its own challenge, as the existing models of scholarly outputs tend to focus on one aspect &mdash; the methods article, the interpretive article or monograph, the database and visual interface. Yet each of these elements was essential for the overall project of this dissertation.

Making this bi-directional argument required that I use a different medium than print. Books, and the historical monograph in particular, operate according to particular genre conventions. While it is possible to subvert those conventions within the print medium &mdash; for example, the literary work of the Oulipo group &mdash; doing so creates a work that is "hard" to read and that provides commentary on the genre itself. Web documents, by contrast, operate according to different conventions &mdash; such as hyperlinking, interactivity, and layering &mdash; that create space for different kinds of argumentation. Because I am pursuing two inter-related arguments in this dissertaton, and relying on data, code, and interactive visualizations to make those arguments, the conventions of web documents are a better fit for the work I am undertaking in the dissertation.

For readability, the dissertation website does mirror some of the conventions of print dissertations. The main content of the dissertation is structured into four chapters, and introduction, conclusion, and the traditional supporting text of a bibliography and acknowledgments. However, although the chapters of this dissertation build sequentially, unlike a traditional narrative history, they are not structured to move forward through time or to unfold as a story. Rather, each chapter provides a different aspect of the overall analysis, and can be read according to the two tracks identified on the [home page](http://dissertation.jeriwieringa.com). 

Additionally, the dissertation leverages the conventions of web documents to expose and connect the layers that make up the analysis of the dissertation. The site contains a collection of code notebooks that document the computational work behind the interpretive analysis as well as an interactive "browser" that provides access to the topic model at the heart of the dissertation. These components are linked to from within the essays to expose the underlying computational analysis or can be explored independently for readers interested primarily in the methodological argument of the dissertation.

As this dissertation relies on different conventions that traditional narrative texts, the interfaces require some explanation. The dissertation can be read in a number of ways. First, it can be read according to either of the two tracks identified on the website home page: "Ellen White and Gender in Seventh-day Adventism" for readers interested in the historical interpretation or "Computational Methods in History" for readers interested in the methodological argument of the dissertation. Additionally, the project can be read according to the links in the top navigation, which guide the reader from the topic model brower, to the essays, code, and conclusions. Each of these elements is introduced below to provide the reader with an explanation of how the piece fits within the overall argument of the dissertation.

## Topic Model Browser

At the core of the project is the browser of the topic model of the SDA literature, accessible at [http://browser.dissertation.jeriwieringa.com](http://browser.dissertation.jeriwieringa.com). This model, built using MALLET and visualized using Andrew Goldstone's [DfR Browser](https://agoldst.github.io/dfr-browser/), provides a window onto the language used across the corpus of Seventh-day Adventist texts that I assembled. The interface is organized according to my interpretation of those topics, as reflected in the topic labels. I discuss my interpretive process for creating the labels in [chapter three](link://slug/chapter-3).

## Essays 

The four essays that make up the primary text of the dissertation establish the context for and interpreting the data from the model. These essays build on one another and together offer the argument of the dissertation in a more traditional narrative form. 

The first chapter, ["The Emergence of Seventh-day Adventism,"](link://slug/chapter-1) provides an overview of Seventh-day Adventism in light of standard accounts of nineteenth-century religion and culture. This chapter is aimed at the reader who is unfamiliar with the context of American religious history or the particulars of the SDA, providing the necessary context for the interpretations forwarded throughout the rest of the dissertation. 

The second chapter, ["Constructing Computational Models from Historical Texts,"](link://slug/chapter-2) provides methodological arguments for the sources, processing, modeling, and interpretive aspects of the project. This chapter is the most technical in content, tying the computational work to the historical interpretation. 

The third chapter, ["Anticipating the End of Time,"](link://slug/chapter-3) establishes the problem of time within early Seventh-day Adventism and uses the topic model to identify three major cycles of end-times expectation during the first seventy years of the denomination's history. A case study on using topic models to identify and reveal overarching trends in a corpus for historical analysis, I trace the prevalence of "end-times" topics over time.

The fourth and final chapter, ["The Gendered Work of Salvation at the End of Time,"](link://slug/chapter-4) builds on the structure of time identified in chapter three to argue that the belief in the impending end of time created space for the development of a culture that was in tension with surrounding norms. The nearness of the second coming necessitated that men and women cooperate in the work of salvation, both within the home and in the missionary activities of the church. 

## Notebooks

As a project based on the computational analysis of text, a large portion of the intellectual and scholarly work the make up the dissertation exists in code. In considering the methodological processes around the use of computational analysis in history, this dissertation makes the claim, both explicitly and implicitly, that this technical work is of central importance to the scholarly object of the dissertation. It does this through the inclusion of code and data files in a collection of [notebooks](link://slug/notebooks-overview), which document the computational work that went into creating and interpreting the topic model. 

Where traditional methods of review rely on the use of clear and well formatted footnotes so that the trail of evidence can be retraced and evaluated, the review of computational driven work requires the use of documented and accessible code, so that both the execution of the techniques and the assumptions embedded within the technical choices, can be seen and evaluated. The code elements can be viewed through the dissertation's web interface, or can be downloaded and run either for verification or for adaptation to other projects. The work of making the technical elements of the dissertation visible and extensible is key to establishing processes for validating computationally-based scholarship in the humanities, an extension of the push for reproducible research in the sciences. 

## About - Process Statement and Bibliography

The final element of the dissertation is the [process statement](link://slug/about), which provides documentation for the different components of the projects, including the final website, the model browser, and the dissertation sources. Per the [requirements of the Department of History and Art History at George Mason University](http://historyarthistory.gmu.edu/graduate/phd-history/digital-dissertation-guidelines), I provide an account of the methods and technologies used in the creation of the dissertation in the process statement. 

I also provide a bibliography of the primary, secondary, and computational tools used in the dissertation. This includes a full listing of the periodical issues included in creating the topic model. Together, all of these aspects of the project constitute the body of work that is *A Gospel of Health and Salvation*.