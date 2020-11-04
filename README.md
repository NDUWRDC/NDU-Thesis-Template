# Ndejje University LaTeX Template for Research Reports

## Purpose
This set of files provides a template that can be used by all levels of students to write their paper in LaTeX. 
Some advantages of using the template are:
* Authors can focus on content, since the correct style is automatically applied.
* The desired citation-style is used throughout and can easily be changed for the entire document.
* The required structure is prepared and authors can add content to chapters right away.
* Uniform linking within the document makes it easier to directly jump to sections from the table of content, to listed bibliography, to tables, graphs, images from the text.
* The structure can be easily adapted to meet new requirements for future templates.
* PDFs are produced in the process which simplifies the sharing and printing in comparrison to MS Word files.
* Since LaTeX is purely text, the source files can be easily managed by a version control system like [git](https://git-scm.com/). Using git and an online repository, e.g. [github](https://github.com), makes it possible to collaborate in a team and have the full history of changes of the report. 

## Requirements
[LaTeX](https://www.latex-project.org/) code consists of text files which are used to generate a PDF. Contrary to a What-You-See-Is-What-You-Get program like MS Word, LaTeX is a typesetting system. This means the author focuses on the content and the system to generate a PDF. LaTeX is the de facto standard publication of scientific documents.
### Editor / Environment
Any text editor can be used to write TeX. It is advisable to use an editor that supports TeX syntax. Some editors also have the TeX environment integrated to allow PDF compilation automatically. [Some of many options](https://alternativeto.net/software/texmakerx/) are
- Editors (no environment)
  - [TeXStudio](https://texstudio.org/) 3.0.1 (November 2020): 375MB on harddrive required. Requires TeXworks.
- Editors with environment
  - [Texmaker](https://www.xm1math.net/texmaker/) 5.0.4 (January 2020): 200MB on harddrive required. Also runs from flash (USB)
  - [TeXworks](https://www.tug.org/texworks/) 0.6 (March 2020)
- Online tools - !This template is not tested on those platforms!
  - [Authorea](https://www.authorea.com/)
  - [Overleaf](https://www.overleaf.com/)
### Reference Management Software (optional)
To manage reference dedicated software can be used such as [Zotero](https://www.zotero.org/). This helps to conveniently save the full reference information to a library that in turn integrates to the LaTeX bib-file. 

## Usage
### Editing
Each faculty or department has it's own templates in the root directory. The pattern for the naming is `FacultyReporttype`, e.g. `EngineeringThesis` for the Faculty of Engineering and Survey and the template for Final Year Project Reports.
Download the [latest package](https://github.com/orgs/NDUWRDC/packages?repo_name=NDU-Thesis-Template) from github to a local file.
Edit the following files
* `Macros/Definitions.tex` to change 
  * Faculty name, thesis type, degree type
  * author's names and IDs
  * supervisor(s) names
  * Title and subtitle of report
* `002-FrontMatters/Abstract.tex` to write the abstract.
* `002-FrontMatters/Acknowledgement.tex` to add an acknowledgments section.
* `002-FrontMatters/Dedication.tex` to add a dedication section.
* `003-Acronyms/Acronyms` to add to the list of available acronyms. Acronyms can be used throughout the text. At the firt mention the full name will be given.
* `100-Introduction/Introduction` to write chapter *Introduction*. The chapter already has subsections
  * *Background*
  * *Problem Statement*
  * *Objectives*
  * *Justification*
  * *Scope*
  * *Conceptual Frame Work*
* `200-Literature/Literature` to write chapter *Literature Review*.
* `300-Methodology/Methodology` to write chapter *Methodology*.
* `400-Results/Results` to write chapter *Results*.
* `500-Conclusions/Conclusions` to write chapter *Conclusions*.
* `600-Appendices/Appendices` to add all appendices.
* `Bibliography/references` to have all references available for easy citation in the text.

In addition to the prepared files for chapters, references, and the front matter, the file folder `600-Appendices\Examples` with file `examples.tex` provides demonstrations on how to achieve the most common LaTeX elements such as tables, graphs, charts, pictures, citations, forumulas, abbreviations, symbols, links.

### Version Control
[TortoiseGit](https://tortoisegit.org/) can be used to syncronize with an online repository. That will help to not loose a single version of the report.
