---
layout: post
section-type: post
category: etc
---

## About

[Live Version](https://notes.wilderdan.com)

[GitHub](https://github.com/wilderdan/notebook)

A website I made to share my notes. 
Early in development.

---

## Technical Details

- [Cookie Cutter](https://github.com/cookiecutter/cookiecutter) for creating project template.
- [Jupyter Book](https://jupyterbook.org) as a static site generator.
- GitHub Actions for a CI/CD pipeline.
- MyST markdown (math) syntax for displaying mathematical notation
- Python and numpy for working with matrices
- Created a subdomain

---

## Talk

### Background

I want to study advanced mathematics and computer science.
The highest math classes I took as part of my Computer Science degree were:
- Calculus II
- Linear Algebra 
- Discrete Structures
- Design & Analysis of Algorithms

I considered going back to school to study, but practical concerns such as expenses and my job made me reconsider.
Thus, my self-study plan was born.

I am starting with (Abstract) Algebra through reading Micahel Artin's "Algebra" 2nd edition.
It's been some years since I graduated.
So I will likely be reviewing other material as well.

I've been experimenting with how to take math notes.
I use pen and paper to work through and solve problems.
I then curate and tidy up what I want to save and transfer it over to a Jupyter Notebook.
I also wanted the ability to share and access my notebook over the internet.
Jupyter Book solved that problem. 

### Set Up

I used Cookie Cutter template for a Jupyter Book project. 
This got me up and running quickly.
In particular, it created a `deploy.yml` file for GitHub Actions.
This makes the workflow similar to this website - I push changes to GitHub and it gets built and deployed automatically.
The project structure is self explanatory and was easy to adapt to my purposes.

### What I did

I spent some time learning the markdown necessary to render mathematical notation.
It is fairly straightforward and easy to look up as needed. 
It is much more tedious to type out compared to using pencil and paper.
The positive side is that it looks great.
Especially since my handwriting is pretty terrible.

I read the first chapter which covered Matrices and took notes.
I worked through the first section of exercises on matrices.
I solved some of the problems by hand and others with Python and numpy.
I made sure that I understood the concepts (I could solve by hand) when coding a solution.
I also plan on using Python to display graphs should the need arise.

I only own a single domain name "wilderdan.com", so I figured I would try out using a subdomain "notes" to associate with it. 
All I had to do was create a CNAME record on my Namecheap dashboard,
and configure the settings in the GitHub repository. 

I continue to work on the project locally in VSCodium with the Jupyter extension. 
I build and test locally.
Commit and push changes for that sweet build/deploy.

### Closing Thoughts

I learned a lot.
I hope that this motivates me to continue studying.
However, it is somewhat time consuming to write the mathematical notation.
I will continue to evaluate the effort vs reward.