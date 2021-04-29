# Ndejje University LaTeX Template for BCE Final Year Project Report

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

## Usage
### Editing
Each faculty or department has it's own branch. Currently available:
* [BCE-FYR](https://github.com/NDUWRDC/NDU-Thesis-Template/tree/BCE-FYR) for Civil Engineering Final Year Project Reports
* [BCE-FYR-Proposal](https://github.com/NDUWRDC/NDU-Thesis-Template/tree/BCE-FYR-Proposal) for Civil Engineering Final Year Project Proposals

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
  * *Conceptual Framework*
* `200-Literature/Literature.tex` to write chapter *Literature Review*.
* `300-Methodology/Methodology.tex` to write chapter *Methodology*.
* `400-Results/Results.tex` to write chapter *Results*.
* `500-Conclusions/Conclusions.tex` to write chapter *Conclusions and Recommendations*.
* `600-Appendices/Appendices.tex` to add all appendices.
* `Bibliography/references.bib` to have all references available for easy citation in the text.

In addition to the prepared files for the front matter, chapters, and references, the file folder `600-Appendices\Examples` with file `examples.tex` provides demonstrations on how to achieve the most common LaTeX elements such as tables, graphs, charts, pictures, citations, formulas, abbreviations, symbols, links.

### Create a new repo from template (github)
Logged in at github, browse to https://github.com/NDUWRDC/NDU-Thesis-Template/tree/BCE-FYR and click `Use this template`.
Name the repository, e.g. 'MyThesisName', change to 'private' if required, and click `Create repository from template`.

## Requirements
Contrary to a _What You See Is What You Get_ program like MS Word or OpenOffice/LibreOffice, [LaTeX](https://www.latex-project.org/) is a typesetting system. This means the author focuses on the content and hands over decissions on best typesetting to the system, aka _What You See Is What You Mean_. LaTeX code consists of text files which are used to generate a PDF. To use this template an editor and a LaTeX distribution is required. In addition a reference management system can make live much easier. Finally it is suggested to use a version control system that tracks the evolution of the thesis and allows for collaboration on a centralized document. There are many different [Free and Open Source Softwares](https://en.wikipedia.org/wiki/Free_and_open-source_software) (FOSS) that can be used, some are listed here for a quick orientation.

### Editor / Distribution
Any text editor can be used to write LaTeX. It is advisable to use an editor that supports TeX syntax. Some editors also have the LaTeX environment integrated to allow PDF compilation automatically. [Some of many options](https://alternativeto.net/software/texmakerx/) are
- Editors / Integrated writing environment
  - Editors dedicated to LaTeX
	  - __[TeXStudio](https://texstudio.org/) 3.0.1__ (November 2020), also available as a [portable version](https://www.texstudio.org/#download).
	  - [TeXmaker](https://www.xm1math.net/texmaker/) 5.0.4 (January 2020), also runs from flash (USB).
	  - [TeXworks](https://www.tug.org/texworks/) 0.6 (March 2020)
  - General purpose editors with 'LaTeX modules'
  	- [VS Code](https://code.visualstudio.com/) or it's FOSS equivalent [VSCodium](https://vscodium.com/) 1.51.1 (November 2020)\
	 Use the zip-file (VSCodium-win32-x64-x.yy.z.zip) to [create a portable version](https://code.visualstudio.com/docs/editor/portable)
	   - [Install extension LaTeX workshop](https://medium.com/@rcpassos/writing-latex-documents-in-visual-studio-code-with-latex-workshop-d9af6a6b2815)
	- [Atom](https://atom.io/) 1.52 (November 2020)\
	To use [Atom as a LaTeX editor](https://pwsmith.github.io/2020/05/30/setting-up-a-text-editor-for-LaTeX/) some packages need to be installed at menu File-Settings-Install and the settings adjusted where necessary. Atom has also [a github package](#install-a-gui) available to allow easy integration.
	    - [atom-latex package](https://atom.io/packages/atom-latex) 0.9.1 (January 2020)
	    - [Spell Check package](https://atom.io/packages/spell-check) 0.76.2 (October 2020)\
	    Settings->Grammars (list of scopes): add `, text.tex.latex`
  
- Distributions
  - __[MiKTeX](https://miktex.org/) 20.11__ (November 2020): 240 MB, also installs TeXworks, also available as [Portable Edition](https://miktex.org/howto/portable-edition).
  	- If not already present [Perl](http://strawberryperl.com/releases.html) 5.32 (August 2020) needs to be installed, portable version is available.
  - [TeX Live](https://tug.org/texlive/) 2020 (April 2020) comes with TeXworks, full install needs 7 GB. Custom installation allows for portable version and smaller size.
- Online tools - !This template is not tested on those platforms!
  - [Authorea](https://www.authorea.com/)
  - [Overleaf](https://www.overleaf.com/)

### Reference Management Software (optional)
To manage references a dedicated software can be used. This helps to conveniently save the full reference information to a library that in turn integrates to the LaTeX bib-file.
- __[Mendeley](https://www.mendeley.com/reference-management/reference-manager)__
  - [Mendeley Reference Manager v2.44.0](https://www.mendeley.com/download-reference-manager) (March 2021)
- [Zotero](https://www.zotero.org/)
  - [Zotero](https://www.zotero.org/download/) 5.0 (November 2020)
  - [Zotero Connector](https://www.zotero.org/download/) for Zotero integration in browser Firefox/Chrome/Safari/Edge
  - [Better BibTeX (BBT)](https://retorque.re/zotero-better-bibtex/) an extension for Zotero, follow the [instructions](https://retorque.re/zotero-better-bibtex/installation/).\
  Zotero can be run together with a [portable edition of Firefox](https://portableapps.com/apps/internet/firefox_portable) using a [portable edition of Zotero](https://github.com/pedrom34/ZoteroPortable/).
- [EndNote basic](https://endnote.com/) (not FOSS)
- [JabRef](https://www.jabref.org/)

### Version Control System (optional)
The usage of a distributed [VCS](https://en.wikipedia.org/wiki/Distributed_version_control) will help to not loose a single version of the report with the option to restore former work and work together in teams. An online repository is syncronized with your local files.
To learn more about LaTeX you can use the [Overleaf documentation](https://www.overleaf.com/learn/latex/Main_Page), it's a great place to see the many possibilities that come with LaTeX. See  also a more detailed [git tutorial for LaTeX projects](https://www.desy.de/~bargheer/gitintro/git.html).

#### Install git
* [Git 2.29.2.2](https://git-scm.com/downloads) (November 2020), a portable git version is available.

#### Install a GUI
There are several Shell Interfaces available for git to make the usage more comfortable, [some examples out of many](https://git-scm.com/download/gui/windows):
* __VSCodium__ already has built-in several git and GitHub extensions to issue git commands from within the editor.
* [Atom GitHub Package](https://atom.io/packages/github) provides a simple way to issue git commands from within the editor. See the [documentation](https://flight-manual.atom.io/using-atom/sections/github-package/).
* [TortoiseGit 2.11.0](https://tortoisegit.org/) (November 2020)
* [GitHub Desktop 2.5.7.0](https://desktop.github.com/) (November 2020)

#### Remote repository
An online repository can be hosted on different providers, sign up to create your own online repository:
* [Github](https://github.com/)
* [Gitlab](https://about.gitlab.com/)
* [Bitbucket](https://bitbucket.org/product)
* [Codegiant](https://codegiant.io/home) or others.

## Software size
The mentioned software packages with their sizes on a flash disk:
|Application|Setup file name|Setup size [MB]|Path on Flash|Size on Flash|
|---|---|---|---|---|
|Git for Windwos|Git-2.29.2.2-64-bit.exe                               |46,29|
|Git portable for Windows|PortableGit-2.29.2.2-64-bit.7z.exe                    |42,57|D:\PortableGit|272,46 |
|VScodium for Windwos|VSCodium-win32-x64-1.51.1.zip                         |85,15|D:\VSCodium-portable|375,53|
|GitHub Desktop for Windows|GitHubDesktopSetup.exe                                |96,04|
|TeXlive for Windows|install-tl-windows.exe                                |18,49|D:\TeXlive-portable|1.775,94|
|MiKTex for Windows|basic-miktex-20.11-x64.exe                            |240,70|D:\miktex-portable|962,94|
|TeXworks for Windows|TeXworks-win-setup-0.6.5-202003252107-git_649699a.exe |15,50|
|TeXstudio for Windows|texstudio-3.0.1-win-qt5.exe                           |92,19|
|TeXstudio portable for Windows|texstudio-3.0.1-win-portable-qt5.zip                  |95,31|D:\texstudio-portable|390,09|
|Atom for Windows|AtomSetup-x64.exe                                     |171,92|
|Perl portable for Windows|strawberry-perl-5.32.0.1-64bit-portable.zip           |149,14|
|Zotero for Windows|Zotero-5.0.93_setup.exe                               |40,70|
|Zotero portable for Windows|ZoteroPortable_5.0_Development_Test_67.paf.exe        |45,49|D:\ZoteroPortable|172,31|
|Zotero BetterBibTex Addon for Zotero|zotero-better-bibtex-5.1.133.xpi                      |20,14|
|Firefox portable for Windows|FirefoxPortable_82.0.3_English.paf.exe                |113,16|D:\FirefoxPortable|666,94|
|Firefox Zotero Addon for Windows|Zotero_Connector-5.0.76.xpi                           |0,84|
