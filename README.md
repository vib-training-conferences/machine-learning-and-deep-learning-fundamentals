<!--
author:   Heyse Jolan
email:    trainingandconferences@vib.be
version:  0.0.1
language: en
narrator: UK English

icon:     https://vib.be/sites/vib.sites.vib.be/files/logo_VIB_noTagline.svg

comment:  This document shall provide an entire compendium and course on the
          development of Open-courSes with [LiaScript](https://LiaScript.github.io).
          As the language and the systems grows, also this document will be updated.
          Feel free to fork or copy it, translations are very welcome...

script:   https://cdn.jsdelivr.net/chartist.js/latest/chartist.min.js
          https://felixhao28.github.io/JSCPP/dist/JSCPP.es5.min.js

link:     https://cdn.jsdelivr.net/chartist.js/latest/chartist.min.css
link:     https://cdnjs.cloudflare.com/ajax/libs/animate.css/4.1.1/animate.min.css
link:     https://raw.githubusercontent.com/vib-tcp/material-liascript/master/img/org.css
link:     https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.11.2/css/all.min.css
link:     https://fonts.googleapis.com/css2?family=Saira+Condensed:wght@300&display=swap
link:     https://fonts.googleapis.com/css2?family=Open+Sans&display=swap

link:  https://raw.githubusercontent.com/vib-tcp/material-liascript/master/vib-styles.css

@orcid: [@0](@1)<!--class="orcid-logo-for-author-list"-->

@edition:  1st 
@CourseTitle: Machine Learning and Deep Learning Fundamentals

@JSONLD
<script run-once>
  let json = @0 

  const script = document.createElement('script');
  script.type = 'application/ld+json';
  script.text = JSON.stringify(json);

  document.head.appendChild(script);

  // this is only needed to prevent and output,
  // as long as the result of a script is undefined,
  // it is not shown or rendered within LiaScript
  console.debug("added json to head")
</script>
@end

-->

# @CourseTitle

<section>

Hello and welcome to our workshop! We are very happy to have you here.

This is the @edition edition of this workshop, jointly organised by VIB and ELIXIR.

> We are using the interactive Open Educational Resource online/offline course infrastructure called LiaScript.
> It is a distributed way of creating and sharing educational content hosted on github.
> To see this document as an interactive LiaScript rendered version, click on the
> following link/badge: [LiaScript](https://liascript.github.io/course/?https://raw.githubusercontent.com/vib-tcp/training_material_template/main/README.md)

## General context

Machine learning and deep learning are transforming research by enabling data-driven discoveries and predictive modeling. For many researchers, these techniques can unlock new insights from complex datasets, but getting started can feel overwhelming. 

This two-day workshop is designed for researchers with little or no prior experience in machine learning who want to apply these methods in their own work. Through a mix of clear explanations and hands-on exercises in Jupyter notebooks, participants will learn how to process data, build regression and classification models, and train neural networks and convolutional neural networks. 

By the end of the training, you will understand the fundamentals of machine learning and deep learning and gain practical skills to start applying these techniques to your research projects.

## Proposed Schedule

Schedule day 1:

- 9:00 - 9:30 - Welcome and set-up
- 9:30 - 10:45 - Introduction to machine learning
- 10:45 - 11:00 - Coffee break
- 11:00 - 12:30 - Regression
- 12:30 - 13:30 - Lunch break
- 13:30 - 15:00 - Classification
- 15:00 - 15:15 - Coffee break
- 15:15 - 17:00 - Model selection

Schedule day 2:

- 9:00 - 10:45 - Introduction to neural networks
- 10:45 - 11:00 - Coffee break
- 11:00 - 12:30 - Deep neural networks
- 12:30 - 13:30 - Lunch break
- 13:30 - 15:00 - Convolutional neural networks
- 15:00 - 15:15 - Coffee break
- 15:15 - 16:45 - Advanced deep learning topics
- 16:45 - 17:00 - Wrap-up

</section>

# Lesson overview

> <i class="fa fa-lock"></i> **License:** [Creative Commons Attribution 4.0 International  License](https://creativecommons.org/licenses/by/4.0/deed.en)
>
> <i class="fa fa-user"></i> **Target Audience:** Researchers, trainers, training providers
>
> <svg xmlns="http://www.w3.org/2000/svg" height="14" width="16" viewBox="0 0 576 512"><!--!Font Awesome Free 6.5.1 by @fontawesome - https://fontawesome.com License - https://fontawesome.com/license/free Copyright 2023 Fonticons, Inc.--><path d="M384 64c0-17.7 14.3-32 32-32H544c17.7 0 32 14.3 32 32s-14.3 32-32 32H448v96c0 17.7-14.3 32-32 32H320v96c0 17.7-14.3 32-32 32H192v96c0 17.7-14.3 32-32 32H32c-17.7 0-32-14.3-32-32s14.3-32 32-32h96V320c0-17.7 14.3-32 32-32h96V192c0-17.7 14.3-32 32-32h96V64z"/></svg> **Level:** Beginner
>
> <i class="fa fa-arrow-left"></i> **Prerequisites**   
> 1. Familiarity with Python will be required (recommended course: [Programming in Python: master your first project](https://training.vib.be/all-trainings/programming-python-master-your-first-project))
> 2. No prior machine learning experience required
>
> <i class="fa fa-bookmark"></i> **Description**  This course consist of .....
> 
> <i class="fa fa-arrow-right"></i> **Learning Outcomes:**  
> By the end of the course, learners will be able to:
>
> 1. Explain the fundamental concepts of machine learning and deep learning
> 2. Apply data preprocessing techniques such as handling missing values, scaling features, and splitting datasets
> 3. Implement regression and classification models with scikit-learn and evaluate their performance using appropriate metrics
> 4. Construct simple neural networks and convolutional neural networks with PyTorch framework
> 5. Identify issues with model behavior, like overfitting, and adopt solutions such as regularization or dropout
> 6. Interpret the results of machine learning and deep learning models to make informed decisions for research applications 
>
>
> <i class="fa fa-hourglass"></i> **Time estimation**: 2 days
>
> <i class="fa fa-asterisk"></i> **Requirements:** To follow this course and do the exercices, you need to have [Python](https://www.python.org/downloads/) installed on your computer, and be able to run [Jupyter Notebook](https://jupyter.org/) files. 
>
> <i class="fa fa-envelope-open-text"></i> **Supporting Materials**:
> 
> 1. [Exercises and solutions](link)
> 2. [Slides](https://liascript.github.io/course/?https://raw.githubusercontent.com/vib-tcp/training_material_template/refs/heads/main/supplementary/chapter_01_presentation.md)  
> 
> <i class="fa fa-life-ring"></i> **Acknowledgement**:
>
> * [ELIXIR Belgium](https://www.elixir-belgium.org/)
> * [VIB Technologies](https://www.vib.be/)
>
> <i class="fa fa-money-bill"></i> **Funding:** This project has received funding from the ELIXIR Programme 2022-2023.
>
> <i class="fa fa-anchor"></i> **PURL**:  


# Authors and Contributors

Authors

- @[orcid(Jolan Heyse)](https://orcid.org/0000-0003-2179-0366)


## Citing this lesson

Please cite as:
Jolan Heyse, Machine Learning and Deep Learning Fundamentals (VIB Training)

# Chapters List

| Chapter | Title                                                   |
| :---- | :------------------------------------------------         |
| 1     | [Introduction to machine learning](link)                  |
| 2     | [Regression](link)                                        |
| 3     | [Classification](link)                                    |
| 4     | [Model selection](link)                                   |
| 5     | [Introduction to neural networks](link)                   |
| 6     | [Deep neural networks](link)                              |
| 7     | [Convolutional neural networks](link)                     |
| 8     | [Advanced deep learning topics](link)                     |


# References

Here are some great tips for learning and to get inspired for writing your own pipelines:

- Scikit-learn's official documentation ([link](https://scikit-learn.org/stable/index.html))
- Pytorch's official documentation ([link](https://docs.pytorch.org/tutorials/?_gl=1*1drqazn*_up*MQ..*_ga*MTEwMDYxMDMyOC4xNzY4MjEyMTc2*_ga_469Y0W5V62*czE3NjgyMTIxNzUkbzEkZzAkdDE3NjgyMTIxNzUkajYwJGwwJGgw))

# About us

*About ELIXIR Training Platform*

The ELIXIR Training Platform was established to develop a training community that spans all ELIXIR member states (see the list of Training Coordinators). It aims to strengthen national training programmes, grow bioinformatics training capacity and competence across Europe, and empower researchers to use ELIXIR's services and tools.

One service offered by the Training Platform is TeSS, the training registry for the ELIXIR community. Together with ELIXIR France and ELIXIR Slovenia, VIB as lead node for ELIXIR Belgium is engaged in consolidating quality and impact of the TeSS training resources (2022-23) (https://elixir-europe.org/internal-projects/commissioned-services/2022-trp3).

The Training eSupport System was developed to help trainees, trainers and their institutions to have a one-stop shop where they can share and find information about training and events, including training material. This way we can create a catalogue that can be shared within the community. How it works is what we are going to find out in this course.

*About VIB and VIB Technologies*

VIB is an entrepreneurial non-profit research institute, with a clear focus on groundbreaking strategic basic research in life sciences and operates in close partnership with the five universities in Flanders – Ghent University, KU Leuven, University of Antwerp, Vrije Universiteit Brussel and Hasselt University.

As part of the VIB Technologies, the 12 VIB Core Facilities, provide support in a wide array of research fields and housing specialized scientific equipment for each discipline. Science and technology go hand in hand. New technologies advance science and often accelerate breakthroughs in scientific research. VIB has a visionary approach to science and technology, founded on its ability to identify and foster new innovations in life sciences.

The goal of VIB Technology Training is to up-skill life scientists to excel in the domains of VIB Technologies, Bioinformatics & AI, Software Development, and Research Data Management.

--------------------------------------------

*Editorial team for this course*

Authors: @[orcid(Jolan Heyse)](https://orcid.org/0000-0003-2179-0366), @[orcid(Bruna Piereck)](https://orcid.org/0000-0001-5958-0669), @[orcid(Alexander Botzki)](https://orcid.org/0000-0001-6691-4233)

Technical Editors: Jolan Heyse

License: [![CC BY SA](img/picture003.jpg)](https://creativecommons.org/licenses/by-sa/4.0/deed.en)

```json   @JSONLD
{
  "@context": "https://schema.org/",
  "@type": "LearningResource",
  "@id": "https://elixir-europe-training.github.io/ELIXIR-TrP-TeSS/",
  "http://purl.org/dc/terms/conformsTo": {
    "@type": "CreativeWork",
    "@id": "https://bioschemas.org/profiles/TrainingMaterial/1.0-RELEASE"
  },
  "description": "Machine Learning and Deep Learning Fundamentals; This is our interactive hands-on course about the fundamental principles of machine learning and deep learning.",
  "keywords": "Machine learning, Deep learning, Artificial intelligence",
  "name": "Machine Learning and Deep Learning Fundamentals",
  "license": "https://creativecommons.org/licenses/by/4.0/",
  "educationalLevel": "beginner",
  "competencyRequired": "none",
  "teaches": [
    "Explain the fundamental concepts of machine learning and deep learning",
    "Apply data preprocessing techniques such as handling missing values, scaling features, and splitting datasets",
    "Implement regression and classification models with scikit-learn and evaluate their performance using appropriate metrics",
    "Construct simple neural networks and convolutional neural networks with PyTorch framework",
    "Identify issues with model behavior, like overfitting, and adopt solutions such as regularization or dropout",
    "Interpret the results of machine learning and deep learning models to make informed decisions for research applications"
  ],
  "audience": "researchers, training providers",
  "inLanguage": "en-US",
  "learningResourceType": [
    "tutorial"
  ],
  "author": [
    {
      "@type": "Person",
      "name": "Jolan Heyse"
    }
  ],
  "contributor": [
    {
      "@type": "Person",
      "name": "Jolan Heyse"
    },
    {
      "@type": "Person",
      "name": "Bruna Piereck"
    },
    {
      "@type": "Person",
      "name": "Alexander Botzki"
    }
  ]
}
```










