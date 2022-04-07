
# Documentation
Documentation system using markdown and converting to PDF


Experimental repo to test ideas of using markdown to create documentation files and using pandoc and templates to generate PDF files.

The pandoc github has some examples of using github workflows to automate this inside github. I want to experiment with using this to generate the PDF and to then publish it perhaps back in to the repo.

See here: https://github.com/pandoc/pandoc-action-example/tree/master

I've taken the advanced task in the example workflow and copied it in to the workflow in this repo.

Running that workflow is able to generate an artifact (the PDF) which can be downloaded from here:
https://github.com/JohnRyland/Documentation/suites/5971292119/artifacts/205389030

previous version here:
https://github.com/JohnRyland/Documentation/suites/5970774333/artifacts/205358976


This artifact will expire soon. It seems that the available artifacts can be queried with a github API:

curl -H "Accept: application/vnd.github.v3+json" https://api.github.com/repos/JohnRyland/Documentation/actions/artifacts

This lists them. It would be good to be able to list them by branch so as to have a release branch that has artifacts with longer expiries.


This repo is going to be a playground for ideas about project documentation.

I might also experiment with doing something similar with doxygen comments in code and seeing how this can be integrated with github workflows.

Also want to test out plantUML integration in github. I have locally used gitbucket (similar to github and bitbucket) where I have played with different ways to add plantUML in to markdown documents and have it displayed. I want see what is possible in github. Ideally the plantUML can be embedded directly in to the document without needing to keep the plantUML in a seperate file. Similar to this, I want to see if the same is possible with maths equations, and then on top of all this, if this can all be generated in to the PDF file by pandoc.


