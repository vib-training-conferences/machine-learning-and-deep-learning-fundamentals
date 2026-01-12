<!--
author:   Heyse Jolan
email:    trainingandconferences@vib.be
version:  0.0.1
language: en
narrator: UK English

icon:     https://vib.be/sites/vib.sites.vib.be/files/logo_VIB_noTagline.svg

comment:  This document provides the full LiaScript source for the
          course.
-->

@CourseTitle: Machine Learning and Deep Learning Fundamentals
@edition: 1st

@JSONLD
<script run-once>
  let json = @0;

  const script = document.createElement('script');
  script.type = 'application/ld+json';
  script.text = JSON.stringify(json);

  document.head.appendChild(script);

  console.debug("added json to head");
</script>
@end

# @CourseTitle

<section>

Hello and welcome to our workshop! We are very happy to have you here.

This is the @edition edition of this workshop, jointly organised by **VIB**.

> We are using the interactive Open Educational Resource infrastructure called **LiaScript**.
> It is a distributed way of creating and sharing educational content hosted on GitHub.
> To see this document as an interactive rendered version, use the following link:
> [LiaScript course view](https://liascript.github.io/course/?https://raw.githubusercontent.com/jolanhey/machine-learning-and-deep-learning-fundamentals/main/course.md)

## General context

Machine learning and deep learning are transforming research by enabling data-driven discoveries and predictive modeling. For many researchers, these techniques can unlock new insights from complex datasets, but getting started can feel overwhelming.

This two-day workshop is designed for researchers with little or no prior experience in machine learning who want to apply these methods in their own work. Through a mix of clear explanations and hands-on exercises in Jupyter notebooks, participants will learn how to process data, build regression and classification models, and train neural networks and convolutional neural networks.

By the end of the training, you will understand the fundamentals of machine learning and deep learning and gain practical skills to start applying these techniques to your research projects.

## Proposed schedule

### Day 1

- 09:00 – 09:30 — Welcome and set-up
- 09:30 – 10:45 — Introduction to machine learning
- 10:45 – 11:00 — Coffee break
- 11:00 – 12:30 — Regression
- 12:30 – 13:30 — Lunch break
- 13:30 – 15:00 — Classification
- 15:00 – 15:15 — Coffee break
- 15:15 – 17:00 — Model selection

### Day 2

- 09:00 – 10:45 — Introduction to neural networks
- 10:45 – 11:00 — Coffee break
- 11:00 – 12:30 — Deep neural networks
- 12:30 – 13:30 — Lunch break
- 13:30 – 15:00 — Convolutional neural networks
- 15:00 – 15:15 — Coffee break
- 15:15 – 16:45 — Advanced deep learning topics
- 16:45 – 17:00 — Wrap-up

</section>

# Lesson overview

> **License:** Creative Commons Attribution 4.0 International (CC BY 4.0)
>
> **Target audience:** Researchers, trainers, training providers
>
> **Level:** Beginner
>
> **Prerequisites:**
> 1. Familiarity with Python (recommended course: *Programming in Python: master your first project*)
> 2. No prior machine learning experience required
>
> **Description:**
> This course introduces the fundamental concepts of machine learning and deep learning, with a strong emphasis on practical application using Python, scikit-learn, and PyTorch.
>
> **Learning outcomes:** By the end of the course, learners will be able to:
> 1. Explain the fundamental concepts of machine learning and deep learning
> 2. Apply data preprocessing techniques such as handling missing values, scaling features, and splitting datasets
> 3. Implement regression and classification models with scikit-learn and evaluate their performance
> 4. Construct simple neural networks and convolutional neural networks with PyTorch
> 5. Identify issues such as overfitting and apply regularization or dropout
> 6. Interpret model results for research applications
>
> **Time estimation:** 2 days
>
> **Technical requirements:**
> - Python installation
> - Ability to run Jupyter Notebooks

# Authors and contributors

## Authors

- Jolan Heyse (ORCID: https://orcid.org/0000-0003-2179-0366)

## Contributors

- Bruna Piereck
- Alexander Botzki

## Citing this lesson

Please cite as:

> Jolan Heyse, *Machine Learning and Deep Learning Fundamentals*, VIB Training.

# Chapters list

| Chapter | Title |
|:--:|:--|
| 1 | Introduction to machine learning |
| 2 | Regression |
| 3 | Classification |
| 4 | Model selection |
| 5 | Introduction to neural networks |
| 6 | Deep neural networks |
| 7 | Convolutional neural networks |
| 8 | Advanced deep learning topics |

# References

- Scikit-learn documentation: https://scikit-learn.org/stable/
- PyTorch tutorials: https://docs.pytorch.org/tutorials/

# About ELIXIR Training Platform

The ELIXIR Training Platform develops a training community across all ELIXIR member states, strengthening national training programmes and empowering researchers to use ELIXIR services and tools.

One service offered by the Training Platform is **TeSS**, the training registry for the ELIXIR community. VIB, as lead node for ELIXIR Belgium, contributes to consolidating quality and impact of TeSS training resources.

# About VIB and VIB Technologies

VIB is an entrepreneurial non-profit research institute focused on strategic basic research in the life sciences, in close partnership with Flemish universities. VIB Technologies and its Core Facilities provide advanced technological support across research domains.

---

```json @JSONLD
{
  "@context": "https://schema.org/",
  "@type": "LearningResource",
  "name": "Machine Learning and Deep Learning Fundamentals",
  "description": "Interactive hands-on course on the fundamentals of machine learning and deep learning",
  "license": "https://creativecommons.org/licenses/by/4.0/",
  "educationalLevel": "beginner",
  "learningResourceType": "tutorial",
  "inLanguage": "en-US",
  "audience": "researchers, training providers",
  "author": [{ "@type": "Person", "name": "Jolan Heyse" }],
  "contributor": [
    { "@type": "Person", "name": "Bruna Piereck" },
    { "@type": "Person", "name": "Alexander Botzki" }
  ]
}
```

