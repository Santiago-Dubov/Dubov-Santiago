---
title: Edulogical 
summary: Machine learning web app built for TO hacks 2021 with the University of Toronto
tags:
- Deep Learning
date: "2020-05-08T17:15:00Z"

# Optional external URL for project (replaces project detail page).
external_link: ""

image: 
  caption: Landing page
  focal_point: Smart

links:
#- icon: twitter
#  icon_pack: fab
#  name: Follow
#  url: https://twitter.com/georgecushen
url_code: "https://devpost.com/software/quizme-e9gnh7?ref_content=my-projects-tab&ref_feature=my_projects"
url_pdf: ""
url_slides: ""
url_video: ""

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
#slides: example
---
An app built by students for students. 
## 💡 Inspiration
If the pandemic has shown us anything, it's that technology can have an incredibly positive impact on our lives and we haven't even begun to scratch the surface on the possibilities out there. NLP has advanced at breakneck pace recently with the invention of transformers and we now have the possibility to use machine learning very effectively to aid students in their learning. With students under increased pressure to not only achieve good grades but also take part in personal projects and apply to internships, any tools that can help us be better learners are most welcome. 

We started off with a question, what part of the studying experience can be tedious? What machine learning technology could we use to improve this? This ultimately led us to our solution: **EduLogical**. 

## 🔍 What it does

EduLogical is a web app that allows students to improve their retention of key information. Improving test scores and overall understanding through distillation of key ideas. 

**Summarize:** Users can upload a pdf document which will be reduced to down to a concise summary that students can study from instead.

**Create:**  We then generate a quiz based on these summaries that contains a variety of different type of questions. The quiz is stored on the user's account for easy access.


## 🏠 How we built it
* **Frontend:** We used React + HTML + CSS

* **Backend:** We used Cockroach DB, openAI, as well as HuggingFace API

* **Machine Learning:** Bart-Large CNN for the summarization as well as the OpenAI API and a T5 pipeline for question generation. We used glove word embeddings to obtain related (but incorrect) answers for the multiple choice questions. 

## 🛑 Challenges we ran into
* Converting a pdf into text (it's harder than it sounds!) - Sometimes different PDF sections don't translate well, as well multi column structures. Spaces can get lost, as well as unique characters.
* Summarizing - It's difficult to summarize just the right amount and the right quality, it takes a lot of tinkering with AI in the back to get good results!
* Creating the machine learning pipeline 
* Integration is by far the most difficult part and we absolutely ran out of time

## ✅ Accomplishments that we're proud of
* Summarizing a long Biology text well
* Recognizing the benefits of summarizing paragraph by paragraph instead of page by page
* Getting two ML APIs to work well with our system
* Generating sensible multiple choice questions from important points in the summary
* Generating context aware alternative answers for multiple choice questions (harder than it sounds!)

## 📚 What we learned
* 40% of the work for machine learning goes into conceptually dividing and organizing the problem in a way that makes sense for machine learning
* Another 40% of the work goes into optimizing the results by tuning parameters or reformatting the data
* Only 20 % of the work goes into actually coding machine learning 
* Making things connect in the back is hard!

## 🛫 What's next for QuizMe
* Probably build a super AI and take over the world 
* Look into some business case analysis and potentially fine tuning and hosting for real use.