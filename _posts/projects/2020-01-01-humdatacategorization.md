---
layout: project
permalink: /:title/
category: projects

meta:
  keywords: "Humanitarian data, machine learning"

project:
  title: "Automated Humanitarian Data Classification"
  type: "humanitarian, machine learning"
  url: ""
  logo: "/assets/images/projects/humdata/humdata1.png"
  tech: "HTMl, CSS, Javascript"

agency:
  title: "Humanitarian Data Exchange"
  url: "https://data.humdata.org/"
  year: "2021"

images:
  - image:
    url: "/assets/images/projects/humdata/humdata2.png"
  - image:
    url: "/assets/images/projects/humdata/humdata3.png"
  - image:
    url: "/assets/images/projects/humdata/humdata4.png"
  - image:
    url: "/assets/images/projects/humdata/humdata5.png"

---
<p>The objective of this framework is to detect, classify, and recommend a category of data in the context of natural disasters and humanitarian emergencies. The categories of humanitarian data collected during an onset of a crisis is usually limited to the most immediate needs of a population. By identifying these categories and classifying incoming data, humanitarians and information managers can focus on collecting, cleaning, and utilizing information while automatically classified data is analyzed and mapped.</p>
<br>
<p>Over 2,000 datasets were scraped from the Humanitarian Data Exchange (HDX). The datasets pulled had Humanitarian Exchange Language (HXL) tags, which identify the type of data. This data was processed and distilled down to a certain number of tags that are only relevant to rapid needs assessments. These tags were then turned into categories for a training set for our model.Word embeddings were created using fastText, an NLP library created by Facebook. An MLP model is then trained using these word embeddings.</p>
<br>
<p>Assorted rapid needs assessment datasets are then tested to see the model's accuracy.</p>
<br>
