### Data Management and Reproducible Research - 2016.10.27 - Dan Lurie and Chris Gagne

Another scientist should be able to reproduce your entire research pipeline, from data collection to final figures, without having to email you with questions. It sounds intimidating, but it doesn't have to be, and in practice it's usually not that much extra work. You already know all the information they would need, it's largely just a matter of being mindful of how you do things and keeping a record. More selfishly, working in a reproducible way will make your own life easier, especially when you have to come back to a project months or years later.

### Practical Guidelines for Reliable and Reproducible Research
- Protect the sanctity of your raw data.
	- Always keep a hard-copy backup (e.g. CD/DVD, jump drive).
	- Thou shalt not modify. Make copies instead.
	- If working on a shared computer, lock down file permissions.
- Keep things organized!
	- Folder and file names should be self explanatory.
	- Be descriptive! You’re not paying per character.
	- If possible, use a standardized file structure (e.g. [Brain Imaging Data Structure](http://bids.neuroimaging.io/)).
	- Track [data provenance](https://en.wikipedia.org/wiki/Provenance#Data_provenance). Where did this file come from?
	- Use [README files](https://en.wikipedia.org/wiki/README) to store notes about the contents of each folder.
- Keep a lab notebook.
	- Track everything you do in your research. You're not going to remember later.
	- What manual edits or manipulations did you make to the data (and why)?
	- What commands did you run, in what order, and with what options?
	- What did you try that didn’t work?
- Have a backup plan.
	- Dropbox and Google Drive are crazy easy to use.
	- Make sure data is properly anonymized before uploading anywhere!
	- Think about long-term storage options. What happens when you leave the lab?
- Use a version control system (e.g. [GitHub](https://github.com/)) to track changes.
	- Unlimited private GitHub repositories with the free [Student Developer Pack](https://education.github.com/pack).
	- Not just for code! Upload your data too.
	- [SparkleShare](https://www.sparkleshare.org/) lets you use GitHub without having to run any commands.
	- You can also edit most files directly through the GitHub web interface.

### Using GitHub for Version Control

Learning resources:
- [Git Basics - What is version control? (video)](https://git-scm.com/video/what-is-version-control)
- [The Git Parable](https://practical-neuroimaging.github.io/git_parable.html)
- [Git/Github: A primer for researchers](https://datapub.cdlib.org/2014/05/05/github-a-primer-for-researchers/)
- [A quick introduction to version control with Git and GitHub](https://www.authorea.com/users/5990/articles/17489/_show_article)
- [Git for scientists: A tutorial](http://nyuccl.org/pages/gittutorial/)
- [Version control with Git](http://swcarpentry.github.io/git-novice/)

Basic GitHub workflow:

1. Initialize a project repository.
2. Add files.
3. Commit changes.
4. Push changes.
5. Repeat steps 2-4 as you work.

### Digital Lab Notebooks

For some reason, many in psychology and neuroscience seem to have forgotten about [lab notebooks](https://en.wikipedia.org/wiki/Lab_notebook). In almost every other area of science, lab notebooks sit at the very core of the entire research enterprise. It's not just a log of what you've done, it's also a place to make plans, consider hypotheses, jot down half formed ideas, etc. Science isn't just the stuff we do when working with subjects or running statistical tests; everything that happens in between is often just as (or even more) important. In recent years, many people have been [moving from paper and pencil to digital lab notebooks](http://www.nature.com/naturejobs/science/articles/10.1038/nj7493-523a), and some scientists are now keeping completely [open notebooks that anyone can view](http://onsnetwork.org/what-is-open-notebook-science/).

We both (Dan and Chris) tend to work in two parallel notebook-type places:

1. A text-based system for research notes, brainstorming, planning, interpretation, daily logs, code snippets, etc. 
2. A computational notebook for doing and tracking our analysis.

Popular text-based systems:
- Evernote
- Google Docs
- [Microsoft OneNote](https://www.onenote.com/)

The concept of a computational lab notebook gained popularity in large part due to the [success of IPython Notebook](http://blog.fperez.org/2012/01/ipython-notebook-historical.html) (now part of Jupyter), but there are now notebook options for most analysis environments.
- [Jupyter](http://jupyter.org/) (supports Python, R, and MATLAB)
- [RStudio and R Markdown](http://rmarkdown.rstudio.com/)
- [MATLAB Live Editor](https://www.mathworks.com/products/matlab/live-editor/)
- [SPSS Syntax Editor](http://williammurrah.com/reproducible-research-and-statistical-analyses/) (not really a notebook, but it will do in a pinch if you have no choice but to use SPSS)

#### Benefits of Keeping a Digital Lab Notebook

**A log of what you did and how you did it.**
This is historically the most important purpose of a lab notebook, and has become even more critical in light of the ["reproductibility crisis"](http://www.nature.com/news/reproducibility-1.17552). If you're good about keeping all your analysis in a notebook, your science will be immediately reproducible and your methods sections will write themselves. Trust us, you're not going to remember all the details later, and one of those little details might make all the difference. 

**A way of sharing results with collaborators.**
Most science is a team sport, and that often means sharing data, results, and analyses with people who may not be in the same place as you. If you use one of the computational notebooks listed above, it is super easy to generate nice looking PDFs or even interactive webpages where collaborators can see the data, analysis code, results and figures.

**A part of your published research.**
More and more journals (even [Nature](http://www.nature.com/authors/policies/availability.html) and [Science](http://www.sciencemag.org/authors/science-editorial-policies)) are requiring authors to publish or provide their raw data and analysis scripts. This is great for science, but can be a pain for scientists if they haven't been doing things in a reproducible way. If you've already got everything in a digital lab notebook and tracked through a GitHub repository, all you have to do is make things public.  

Here are some examples of notebooks/repositories for published/in-press papers:
- [Adaptive engagement of cognitive control in context-dependent decision-making.](https://github.com/mwaskom/Waskom_CerebCortex_InPress)
- [Frontoparietal representations of task context support the flexible control of goal-directed cognition.](https://github.com/mwaskom/Waskom_JNeurosci_2014)
- [Choosing prediction over explanation in psychology: Lessons from machine learning](https://github.com/tyarkoni/PPS2016)
- [Adolescence is associated with genomically patterned consolidation of the hubs of the human brain connectome](https://github.com/KirstieJane/NSPN_WhitakerVertes_PNAS2016)


#### Sharing Notebooks
- GitHub will automatically render any [Jupyter](http://blog.jupyter.org/2015/05/07/rendering-notebooks-on-github/) and [R Markdown](http://rmarkdown.rstudio.com/github_document_format.html) notebooks you have uploaded.
- Use [nbviewer](https://nbviewer.jupyter.org/) to display Jupyter notebooks hosted on your own server.
- Turn a Jupyter notebook into a PDF or HTML website using [nbconvert](https://github.com/jupyter/nbconvert).
- You can optionally hide your code by using this [Jupyter cell](https://github.com/danlurie/quack/blob/master/jupyter_cell_for_code_folding) or [this nbconvert template](https://github.com/danlurie/quack/blob/master/custom.tplx).
- Easily create interactive figures with [Plot.ly](https://plot.ly/) (Python, R, and MATLAB) and [MPLD3](http://mpld3.github.io/) (Python).
- Share your entire computational environment (data, software, scripts, notebooks, etc) using [Binder](http://mybinder.org/)! 

#### Open and reproducible science resources at UC Berkeley:
- [Berkeley Institute for Data Science (BIDS)](http://www.bids.berkeley.edu)
- [D-Lab](http://dlab.berkeley.edu/)
- [Berkeley Initiative for Transparency in the Social Sciences (BITSS)](http://www.bitss.org/)
- [Stat 159/259: Reproducible and Collaborative Statistical Data Science](http://www.jarrodmillman.com/stat159-fall2015/)
- Dan is also always happy to chat about this stuff.

#### Other resources:
- [The Center for Open Science](https://cos.io/)
- [The Transparency and Openness Promotion Guidelines](https://cos.io/top/)

#### PLOS Computational Biology “Ten Simple Rules” Collection:
- [Creating a Good Data Management Plan](http://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.1004525)
- [Computational Biologist’s Laboratory Notebook](http://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.1004385)
- [Care and Feeding of Scientific Data](http://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.1003542)
- [Effective Computational Research](http://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.1003506)
- [Reproducible Computational Research](http://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.1003285)
