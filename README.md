# Ndejje University LaTeX Template for Research Reports

## Purpose
This set of files provides a template that can be used by all levels of students to write their paper in LaTeX.
Some advantages of using a LaTeX template are:
* Authors can focus on content, since the correct style is automatically applied.
* Because style and content are separated in different files, it becomes easy to change certain aspects for the complete document, e.g. citation style.
* The required structure is prepared and authors can add content to chapters right away.
* Uniform linking within the document makes it easier to directly jump to sections from the table of content, to listed bibliography, to tables, graphs, images from the text.
* The structure can be easily adapted to meet new requirements for future templates.
* PDFs are produced in the process which simplifies the sharing and printing in comparrison to MS Word files.
* Since LaTeX is purely text, the source files can be easily managed by a version control system like [git](https://git-scm.com/). Using git and an online repository, e.g. [github](https://github.com), makes it possible to collaborate in a team and have the full history of changes of the report.
* LaTeX is the de facto standard publication of scientific documents.

To learn more about LaTeX you can use the [Overleaf documentation](https://www.overleaf.com/learn/latex/Main_Page), it's a great place to see the many possibilities that come with LaTeX.

## Usage
### Editing
Each faculty or department has it's own branch. Currently available:
* [BCE-FYR](https://github.com/NDUWRDC/NDU-Thesis-Template/tree/BCE-FYR) for Civil Engineering Final Year Project Reports
* [BCE-FYR-Proposal](https://github.com/NDUWRDC/NDU-Thesis-Template/tree/BCE-FYR-Proposal) for Civil Engineering Final Year Project Proposals

Download the [latest releases](https://github.com/NDUWRDC/NDU-Thesis-Template/releases) or use the git clone option (see below).
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
  * *Conceptual Framework*
* `200-Literature/Literature.tex` to write chapter *Literature Review*.
* `300-Methodology/Methodology.tex` to write chapter *Methodology*.
* `400-Results/Results.tex` to write chapter *Results*.
* `500-Conclusions/Conclusions.tex` to write chapter *Conclusions and Recommendations*.
* `600-Appendices/Appendices.tex` to add all appendices.
* `Bibliography/references.bib` to have all references available for easy citation in the text.

In addition to the prepared files for the front matter, chapters, and references, the file folder `600-Appendices\Examples` with file `examples.tex` provides demonstrations on how to achieve the most common LaTeX elements such as tables, graphs, charts, pictures, citations, formulas, abbreviations, symbols, links.

### Create a new repo from template (github)
Logged in at github, browse to https://github.com/NDUWRDC/NDU-Thesis-Template/ and click `Use this template`.
Name the repository, e.g. 'MyThesisName', change to 'private' if required, tick 'Include all branches' and click `Create repository from template`. This will [create a repository with the same directory structure and files](https://docs.github.com/en/github/creating-cloning-and-archiving-repositories/creating-a-repository-from-a-template) as the template. 

## Requirements
Contrary to a _What You See Is What You Get_ program like MS Word or OpenOffice/LibreOffice, [LaTeX](https://www.latex-project.org/) is a typesetting system. This means the author focuses on the content and hands over decissions on best typesetting to the system, aka _What You See Is What You Mean_. LaTeX code consists of text files which are used to generate a PDF. To use this template an editor and a LaTeX distribution is required. In addition a reference management system can make live much easier. Finally it is suggested to use a version control system that tracks the evolution of the thesis and allows for collaboration on a centralized document. There are many different [Free and Open Source Softwares](https://en.wikipedia.org/wiki/Free_and_open-source_software) (FOSS) that can be used, some are listed here for a quick orientation.

### Editor / Distribution
Any text editor can be used to write LaTeX. It is advisable to use an editor that supports TeX syntax. Some editors also have the LaTeX environment integrated to allow PDF compilation automatically. [Some of many options](https://tex.stackexchange.com/questions/339/latex-editors-ides) are
- Editors / Integrated writing environment
  - Editors dedicated to LaTeX
	  - __[TeXStudio](https://texstudio.org/) 3.1.2__ (May 2021), also available as a [portable version](https://www.texstudio.org/#download)
	  - [TeXmaker](https://www.xm1math.net/texmaker/) 5.0.4 (January 2020), available as a portable version
	  - [TeXworks](https://www.tug.org/texworks/) 0.6.6 (March 2021), part of MiKTeX and TeXlive distributions.
  - General purpose editors with 'LaTeX modules'
  	- [VS Code](https://code.visualstudio.com/) or it's FOSS equivalent [VSCodium](https://vscodium.com/) 1.56.2 (May 2021)\
	 Use the zip-file (VSCodium-win32-x64-x.yy.z.zip) to [create a portable version](https://code.visualstudio.com/docs/editor/portable)
	   - [Install extension LaTeX workshop](https://medium.com/@rcpassos/writing-latex-documents-in-visual-studio-code-with-latex-workshop-d9af6a6b2815)
	- [Atom](https://atom.io/) 1.52 (November 2020)\
	To use [Atom as a LaTeX editor](https://pwsmith.github.io/2020/05/30/setting-up-a-text-editor-for-LaTeX/) some packages need to be installed at menu File-Settings-Install and the settings adjusted where necessary. Atom has also [a github package](#install-a-gui) available to allow easy integration.
	    - [atom-latex package](https://atom.io/packages/atom-latex) 0.9.1 (January 2020)
	    - [Spell Check package](https://atom.io/packages/spell-check) 0.76.2 (October 2020)\
	    Settings->Grammars (list of scopes): add `, text.tex.latex`
  
- Distributions
  - __[MiKTeX](https://miktex.org/) 21.2__ (April 2021): 243 MB, also installs TeXworks, also available as [Portable Edition](https://miktex.org/howto/portable-edition).
  	- If not already present [Perl](http://strawberryperl.com/releases.html) 5.32 (August 2020) needs to be installed, portable version is available.
  - [TeX Live](https://tug.org/texlive/) 2021 (April 2021) comes with TeXworks, full install needs 7 GB. Custom installation allows for portable version and smaller size. Perl is part of the installation.
- Online tools
  - [Overleaf](https://www.overleaf.com/)
    - Import files to overleaf by uploading the zipped template.
    - Change the 'Main document' (at Menu) to thesis.tex.
  - [Papeeria](https://www.papeeria.com/)
    - Importing the zipped template works
    - Also works as [mobile app](https://m.papeeria.com/)
    - Some packages are not available (pgf-pie). 
    - Large projects may give troubles in the free plan.
  - [CoCalc](https://cocalc.com/doc/latex-editor.html)
    - Importing files to cocalc by uploading the zipped template works but as of May 2021 the \makeglossaries does not work.
  - [Authorea](https://www.authorea.com/) does not work with the template.

### Reference Management Software (optional)
To manage references a dedicated software can be used. This helps to conveniently save the full reference information to a library that in turn integrates to the LaTeX bib-file.
- __[Mendeley](https://www.mendeley.com/reference-management/reference-manager)__ NOT  FOSS
  - [Mendeley Reference Manager v2.44.0](https://www.mendeley.com/download-reference-manager) (March 2021)
- [Zotero](https://www.zotero.org/)
  - [Zotero](https://www.zotero.org/download/) 5.0.96 (May 2021)
  - [Zotero Connector](https://www.zotero.org/download/) for Zotero integration in browser Firefox/Chrome/Safari/Edge
  - [Better BibTeX (BBT)](https://retorque.re/zotero-better-bibtex/) an extension for Zotero, follow the [instructions](https://retorque.re/zotero-better-bibtex/installation/).\
  Zotero can be run together with a [portable edition of Firefox](https://portableapps.com/apps/internet/firefox_portable) using a [portable edition of Zotero](https://github.com/pedrom34/ZoteroPortable/).
- [JabRef 5.2](https://www.jabref.org/) also available as portable version
- [EndNote basic](https://endnote.com/) NOT FOSS

### Version Control System (optional)
The usage of a distributed [VCS](https://en.wikipedia.org/wiki/Distributed_version_control) will help to not loose a single version of the report with the option to restore former work and work together in teams. An online repository is syncronized with your local files.
A more detailed [git tutorial for LaTeX projects](https://www.desy.de/~bargheer/gitintro/git.html).

#### Install git
* [Git 2.29.2.2](https://git-scm.com/downloads) (November 2020), a portable git version is available.

#### Install a GUI
There are several Shell Interfaces available for git to make the usage more comfortable, [some examples out of many](https://git-scm.com/download/gui/windows):
* __[GitHub Desktop 2.8.1](https://desktop.github.com/)__ (May 2021) also has a [portable Version](https://github.com/daemondevin/GitHubDesktopPortable). Comes with it's own git installation.
* VSCodium already has built-in several git and GitHub extensions to issue git commands from within the editor.
* [Atom GitHub Package](https://atom.io/packages/github) provides a simple way to issue git commands from within the editor. See the [documentation](https://flight-manual.atom.io/using-atom/sections/github-package/).
* [TortoiseGit 2.11.0](https://tortoisegit.org/) (November 2020)

#### Remote repository
An online repository can be hosted on different providers, sign up to create your own online repository:
* [Github](https://github.com/)
* [Gitlab](https://about.gitlab.com/)
* [Bitbucket](https://bitbucket.org/product)
* [Codegiant](https://codegiant.io/home) or others.

## Software size
The following software packages are availabel on a flash disk at WRDC.
### LaTeX and TeXstudio

|Application|Setup file name|Setup size|Path on Flash|Size on Flash|
|---|---|---|---|---|
|MiKTex for Windows|basic-miktex-21.2-x64.exe                            |240 MB|/miktex-portable|1 GB|
|TeXstudio portable for Windows|texstudio-3.1.2-win-portable-qt5.zip                  |107 MB|/texstudio-portable|136 MB (a)|
|LanguageTool 5.3|LanguageTool-5.3.zip|187 MB|/texstudio-portable/languagetool-5.3|145 MB (a)
|Perl portable for Windows|strawberry-perl-5.32.0.1-64bit-portable.zip           |149 MB|/perl-portable|132 MB (a)

(a) Some files deleted to reduce on size

&nbsp;
### Mendeley
|Application|Setup file name|Setup size|Path on Flash|Size on Flash|
|---|---|---|---|---|
|Mendeley|Mendeley-Desktop-1.19.8-win32|55 MB| | |

&nbsp;
### Zotero
|Application|Setup file name|Setup size|Path on Flash|Size on Flash|
|---|---|---|---|---|
|Zotero for Windows|Zotero-5.0.96.2_setup.exe                               |41 MB|
|Zotero portable for Windows|ZoteroPortable_5.0_Development_Test_75.paf.exe        |46 MB|/ZoteroPortable|172,31|
|Zotero BetterBibTex Addon for Zotero|zotero-better-bibtex-5.4.15.xpi|33 MB|
|Firefox portable for Windows|FirefoxPortable_88.0.1_English.paf.exe                |114 MB|/FirefoxPortable|402 MB|
|Firefox Zotero Addon for Windows|Zotero_Connector-5.0.85.xpi                           |1 MB|

&nbsp;
### git and GitHub
|Application|Setup file name|Setup size|Path on Flash|Size on Flash|
|---|---|---|---|---|
|GitHub Desktop for Windows|GitHubDesktopSetup-x64.exe|109 MB|/GitHubDesktopPortable|196 MB
