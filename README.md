# Ndejje University LaTeX Template for Research Reports (not official)

## Purpose
This set of files provides a template that can be used by all levels of students to write their paper in LaTeX. 
Some advantages of using a LaTeX template are:
* Authors can focus on content, since the correct style is automatically applied.
* The desired citation-style is used throughout and can easily be changed for the entire document.
* The required structure is prepared and authors can add content to chapters right away.
* Uniform linking within the document makes it easier to directly jump to sections from the table of content, to listed bibliography, to tables, graphs, images from the text.
* The structure can be easily adapted to meet new requirements for future templates.
* PDFs are produced in the process which simplifies the sharing and printing in comparrison to MS Word files.
* Since LaTeX is purely text, the source files can be easily managed by a version control system like [git](https://git-scm.com/). Using git and an online repository, e.g. [github](https://github.com), makes it possible to collaborate in a team and have the full history of changes of the report. 
* LaTeX is the de facto standard publication of scientific documents.

## Requirements
Contrary to a What-You-See-Is-What-You-Get program like MS Word, [LaTeX](https://www.latex-project.org/) is a typesetting system. This means the author focuses on the content and hands over decissions on best typesetting to the the system. LaTeX code consists of text files which are used to generate a PDF.
### Editor / Environment
Any text editor can be used to write LaTeX. It is advisable to use an editor that supports TeX syntax. Some editors also have the TeX environment integrated to allow PDF compilation automatically. [Some of many options](https://alternativeto.net/software/texmakerx/) are
- Editors (no environment)
  - __[TeXStudio](https://texstudio.org/) 3.0.1__ (November 2020): 375MB on harddrive required. Requires TeXworks.
- Editors with environment
  - __[MiKTeX](https://miktex.org/) 20.11__ (November 2020): 240 MB, also installs TeXworks
  - [Texmaker](https://www.xm1math.net/texmaker/) 5.0.4 (January 2020): 200MB on harddrive required. Also runs from flash (USB)
  - [TeXworks](https://www.tug.org/texworks/) 0.6 (March 2020)
- Online tools - !This template is not tested on those platforms!
  - [Authorea](https://www.authorea.com/)
  - [Overleaf](https://www.overleaf.com/)

### Reference Management Software (optional)
To manage references a dedicated software can be used such as [Zotero](https://www.zotero.org/). This helps to conveniently save the full reference information to a library that in turn integrates to the LaTeX bib-file.
- [Zotero](https://www.zotero.org/download/) 5.0 (November 2020)
- [Zotero Connector](https://www.zotero.org/download/) for Zotero integration in browser Firefox/Chrome/Safari/Edge
- [Better BibTeX (BBT)](https://retorque.re/zotero-better-bibtex/) an extension for Zotero, follow the [instructions](https://retorque.re/zotero-better-bibtex/installation/)

### Version Control System (optional)
The usage of a distributed [VCS](https://en.wikipedia.org/wiki/Distributed_version_control) will help to not loose a single version of the report with the option to restore former work and work together in teams. An online repository is syncronized with your local files.

Git installer:
* [Git 2.29.2.2](https://git-scm.com/downloads) (November 2020): 258 MB of free disk space required.

There are several Shell Interfaces available for git to make the usage more comfortable, [some examples out of many](https://git-scm.com/download/gui/windows):
* __[GitHub Desktop 2.5.7.0](https://desktop.github.com/)__ (November 2020)
* [TortoiseGit 2.11.0](https://tortoisegit.org/) (November 2020)

An online repository can be hosted on different providers, sign up to create your own online repository: 
* [Github](https://github.com/)
* [Gitlab](https://about.gitlab.com/)
* [Bitbucket](https://bitbucket.org/product) 
* [Codegiant](https://codegiant.io/home) or others.

## Usage
### Editing
Each faculty or department has it's own templates in the root directory. The pattern for the naming is `<Faculty><Reporttype>.tex`, e.g. `EngineeringThesis.tex` for the Faculty of Engineering and Survey and the template for Final Year Project Reports.
Download the [latest package](https://github.com/orgs/NDUWRDC/packages?repo_name=NDU-Thesis-Template) or use the git clone option (see below).
Edit the following files
* `Macros/Definitions.tex` to change 
  * faculty name, thesis type, degree type,
  * author's names and IDs,
  * supervisor(s) names,
  * title and subtitle of report,
  * date of submission.
* `002-FrontMatters/Abstract.tex` to write the abstract.
* `002-FrontMatters/Acknowledgement.tex` to add an acknowledgments section.
* `002-FrontMatters/Dedication.tex` to add a dedication section.
* `003-Acronyms/Acronyms.tex` to add to the list of available acronyms.
* `100-Introduction/Introduction.tex` to write chapter *Introduction*. The chapter already has subsections
  * *Background*
  * *Problem Statement*
  * *Objectives*
  * *Justification*
  * *Scope*
  * *Conceptual Frame Work*
* `200-Literature/Literature.tex` to write chapter *Literature Review*.
* `300-Methodology/Methodology.tex` to write chapter *Methodology*.
* `400-Results/Results.tex` to write chapter *Results* or *Design*.
* `500-Conclusions/Conclusions.tex` to write chapter *Conclusions*.
* `600-Appendices/Appendices.tex` to add all appendices.
* `Bibliography/references.bib` to have all references available for easy citation in the text.

In addition to the prepared files for the front matter, chapters, and references, the file folder `600-Appendices\Examples` with file `examples.tex` provides demonstrations on how to achieve the most common LaTeX elements such as tables, graphs, charts, pictures, citations, formulas, abbreviations, symbols, links.

### Create a new repo from template (github)
Logged in at github, browse to https://github.com/NDUWRDC/NDU-Thesis-Template and click `Use this template`.
Name the repository, e.g. 'MyThesisName', change to 'private' if required, and click `Create repository from template`.
