---
start:       <!--
title:       Documentation System
subtitle:    Examples using markdown to generate PDFs
copyright1:  Copyright (C) 2022, John Ryland.
copyright2:  All rights reserved.
date:        7th April 2022
contact:     jryland@gmail.com
background:  background.pdf
end:         -->
---


# Introduction

Experimental repo to test ideas of using markdown to create documentation files and using
pandoc and templates to generate PDF files.


Something like or perhaps exactly like this:

  https://github.com/Wandmalfarbe/pandoc-latex-template/


The background.pdf in this directory comes from there.

```
  pandoc-latex-template/examples/page-background/backgrounds/background6.pdf
```


# GitHub Workflows

The pandoc github has some examples of using github workflows to automate this inside github.
I want to experiment with using this to generate the PDF and to then publish it perhaps back in to the repo.


See here:

  https://github.com/pandoc/pandoc-action-example/tree/master


Also the pandoc-latex-template repo has a workflow, however it doesn't use docker to get pandoc,
it instead downloads and extracts it.


See here:

  https://github.com/Wandmalfarbe/pandoc-latex-template/blob/master/.github/workflows/build-examples.yml


I've taken the advanced task in the pandoc-action-example repo's example workflow and copied it
in to the workflow in this repo. Running that workflow is able to generate an artifact (the PDF)
which can be downloaded from here:


  https://github.com/JohnRyland/Documentation/suites/5971292119/artifacts/205389030


previous version here:


  https://github.com/JohnRyland/Documentation/suites/5970774333/artifacts/205358976


This artifact will expire soon. It seems that the available artifacts can be queried with a github API:

```
curl -H "Accept: application/vnd.github.v3+json" https://api.github.com/repos/JohnRyland/Documentation/actions/artifacts
```

This lists them. It would be good to be able to list them by branch so as to have a release branch that has artifacts with longer expiries.


# Ideas

This repo is going to be a playground for ideas about project documentation.

I might also experiment with doing something similar with doxygen comments in code and seeing
how this can be integrated with github workflows.

Also want to test out plantUML integration in github. I have locally used gitbucket (similar
to github and bitbucket) where I have played with different ways to add plantUML in to markdown
documents and have it displayed. I want see what is possible in github. Ideally the plantUML
can be embedded directly in to the document without needing to keep the plantUML in a seperate
file. Similar to this, I want to see if the same is possible with maths equations, and then on
top of all this, if this can all be generated in to the PDF file by pandoc.


