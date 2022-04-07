
# Documentation
Documentation system using markdown and converting to PDF


Experimental repo to test ideas of using markdown to create documentation files and using pandoc and templates to generate PDF files.

The pandoc github has some examples of using github workflows to automate this inside github. I want to experiment with using this to generate the PDF and to then publish it perhaps back in to the repo.

See here: https://github.com/pandoc/pandoc-action-example/tree/master


This is going to be a playground for ideas about project documentation.

I might also experiment with doing something similar with doxygen comments in code and seeing how this can be integrated with github workflows.

Also want to test out plantUML integration in github. I have locally used gitbucket (similar to github and bitbucket) where I have played with different ways to add plantUML in to markdown documents and have it displayed. I want see what is possible in github. Ideally the plantUML can be embedded directly in to the document without needing to keep the plantUML in a seperate file. Similar to this, I want to see if the same is possible with maths equations, and then on top of all this, if this can all be generated in to the PDF file by pandoc.
