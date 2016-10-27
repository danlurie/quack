## Data Management and Reproducible Research - 2016.10.27 - Dan Lurie and Chris Gagne

Another scientist should be able to reproduce your entire research pipeline, from data collection to final figures, without having to email you with questions. It sounds intimidating, but it doesn't have to be, and in practice it's usually not that much extra work. You already know all the information they would need, it's largely just a matter of being mindful of how you do things and keeping a record. More selfishly, working in a reproducible way will make your own life easier, especially when you have to come back to a project months or years later.

### Practical Guidelines for Reliable and Reproducible Research
- Protect the sanctity of your raw data.
	- Always keep a hard-copy backup (e.g. CD/DVD, jump drive).
	- Thou shalt not modify. Make copies instead.
	- If working on a shared computer, lock down file permissions.
- Keep things organized!
	- Folder and file names should be self explanatory.
	- Be descriptive! You’re not paying per character.
	- If possible, use a standard ontology (e.g. [Brain Imaging Data Structure](http://bids.neuroimaging.io/)).
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

Notebooks:
- NBconvert to webpage or PDF for sharing (templates to delete or hide code)
- Log book —> sharing and publication
- Share on github and nbviewer
- Plotly, mpld3

Useful Notebook Tips
- (look for good examples, combine into a tips notebook)
- also: whole example notebooks (if possible)
- code snippets / command reference

Lab Notebooks
- Jupyter
- R Markdown
- MATLAB Live Editor
- SPSS Syntax Editor


Show examples from Dan’s and Chris’s Projects
tunneling to jupyter on NX

jupyter TOC extensions, hiding code extension

example notebooks

Open and reproducible science resources at UC Berkeley:
- [Berkeley Institute for Data Science (BIDS)](http://www.bids.berkeley.edu)
- [D-Lab](http://dlab.berkeley.edu/)
- [Berkeley Initiative for Transparency in the Social Sciences (BITSS)](http://www.bitss.org/)
- [Stat 159/259: Reproducible and Collaborative Statistical Data Science](http://www.jarrodmillman.com/stat159-fall2015/)

Other resources:
- [The Center for Open Science](https://cos.io/)
- [The Transparency and Openness Promotion Guidelines](https://cos.io/top/)

PLOS Computational Biology “Ten Simple Rules” Collection:
- [Creating a Good Data Management Plan](http://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.1004525)
- [Computational Biologist’s Laboratory Notebook](http://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.1004385)
- [Care and Feeding of Scientific Data](http://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.1003542)
- [Effective Computational Research](http://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.1003506)
- [Reproducible Computational Research](http://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.1003285)
