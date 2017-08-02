# book-coding
Book coding course details http://berlin.publishing-school.net/css-books

Each class sits a seperate module, so you can attend single classes.

## Session 1 - Outline 19.7.17

- class objective: 
    - make a PDF book for A6 pamphlet (self covers), impositioned on A4
    - use XHTML/CSS template to learn book coding basics
    - use Vivliostyle in-browser PDF rendering
- course objective: 
    - make PDF book, eBook, Bootstrap alternative W3.CSS and GitHub-pages web book
    - use GitHub as collaborative workspace
    - metadata
    - book design
- class resources: XHTML/CSS template download, Chrome browser, Vivliostyle, Transpect, Atom text editor, GitHub

## Links

Vivliostyle - https://github.com/vivliostyle/vivliostyle

Transpect - http://transpect.github.io/

CSS Paged Media - https://drafts.csswg.org/css-page/

Paged Media about and guides - https://www.print-css.rocks/

Paged Media covers - https://www.pagedmedia.org/a-book-by-its-cover/

https://gitlab.coko.foundation/julientaq/cabbageTreeMethod

HTML learning the basics - https://www.w3schools.com/html/html_basic.asp

HTML_vs._XHTML - https://wiki.whatwg.org/wiki/HTML_vs._XHTML

CSS learning the basics - https://www.w3schools.com/css/default.asp

W3.CSS (Bootstrap alt)  https://www.w3schools.com/w3css/default.asp

## Setup

- Have Chrome installed, add Vivliostyle app, install Atom text editor, download the template and unpack
- Demo the 16 page template (download or fork above)
- Explore the file structure
- Work with XHTML to start with
- Edit the template and add some Mute content http://www.metamute.org/content/proud-to-be-flesh

## Make your PDF

- click the Vivliostyle app icon top right in your browser, select paginate, spreads.
- select print in your browser, standard PDF, margin set to 0 (zero), save. You have your PDF.

## Make Book

Edit XHTML/CSS files in Atom, save, reload in browser, render with Vivliostyle app. Done!

Features well explore:

- book page size @page css
- paragraph
- book title
- cover
- sections and chapters
- table of contents
- images
- footnotes
- headers

# Session #2 26.07.2017 - Making Ebooks Using Transpect Software

Using the same XHTML/CSS file set we can use the free and open source Transpect software made by le-tex (Leipzig) to make different types of eBooks.

Transpect - http://transpect.github.io/

Transpect on GitHub - https://github.com/transpect

Transpect eBook module 'epubtools-frontend' - https://github.com/transpect/epubtools-frontend

Transpect Twitter - https://twitter.com/letexml @letexml

#psberlin book coding template - https://github.com/hybrid-publishing-group/book-coding

## What we will cover in session #2

  - Demo eBook making
  - Install GitHub - file storage and collaboration
  - Download #psberlin templates
  - Install Transpect 'epubtools-frontend' for ebook making
  - Run Transpect on the CLI
  - Make sample book using Mute content from the book 'Proud to be Flesh'
  - Step-by-step guide to eBook making
  - Review Vivliostyle and Transpect multi-format book making

Next session #3 - Responsive Web book making, Multi-channel distribution: PoD, eBook and GitHub!

## Review

Previously we had used Vivliostyle to generate PDFs for screen and print. See previous notes and template files we will continue to use in this session https://github.com/hybrid-publishing-group/book-coding

## Demo Transpect eBook module 'epubtools-frontend'

  - Transpect - http://transpect.github.io/
  - Software downloaded from GitHub - epubtools-frontend https://github.com/transpect/epubtools-frontend
  - using same template set - XHTML/CSS book-coding/ Template2
  - epubtools-frontend running on the CLI

mrc@bethia:~/Github251016/epubtools-frontend$ ./epubconvert ../book-coding/template2/template2.xhtml

  - Generates a book here /home/mrc/Github251016/book-coding/template2/template2.epub
  - View in Calibre or Readium - open eBook

## Installs

### GitHub

  - Create account https://github.com/
  - Install GitHub desktop https://github.com/transpect/epubtools-frontend
  - Trouble shooting, if CLI GitHub needs installing https://help.github.com/articles/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent/

### Book-coding #psberlin templates

  - https://github.com/transpect/epubtools-frontend
  - Screengrabs - view in finder
  - Using GitHub - clone repository
  - Copy Tempate2 folder and work on the copy, rename and rename file inside Template2.xhtml

### Transpect 'epubtools-frontend'

  - Download https://github.com/transpect/epubtools-frontend

### Need Java 1.8 SDK

  - Locate your CLI - SHELL - applications/utilities/Terminal.app, WIN ?
  - Test on CLI: java -version
  - Java™ Platform, Standard Edition Development Kit (SDK) - http://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.html

## Test making eBook

  - Navigate to on the CLI - /epubtools-frontend$ CLI commands cd xxx, cd ../, ls, pwd, ls -la
  - Run command to make eBook ./epubconvert ../book-coding/template2/template2.xhtml

## Make eBook using Mute content

  - Got to http://www.metamute.org/content/proud-to-be-flesh

    - Introduction - Proud To Be Flesh
    - Chapter 1: Introduction - Direct Democracy and its Demons: Web 1.0 to Web 2.0
    - Chapter 2: Introduction - From Net Art to Conceptual Art and Back
    - Chapter 3: Introduction - I, Cyborg: Reinventing the Human
    - Chapter 4: Introduction - Of Commoners and Criminals
    - Chapter 5: Introduction - Organising Horizontally
    - Chapter 6: Introduction - Assuming the Position: Art and/Against Business
    - Chapter 7: Introduction - Under the Net: the City and the Camp
    - Chapter 8: Introduction - Reality Check: Class and Immaterial Labour
    - Chapter 9: Introduction - The Open Work

## File structure and about eBooks

  - file structure
  - parts that make the ebook - copy template folder to amke new books

## About Responsive W3CSS

Alternative to Bootstrap, under consideration - https://www.w3schools.com/w3css/default.asp

## eBook making - step-by-step

## Different outputs

  - Print sizes
  - eBook types

## Review

  - GitHub Issues
  - Slack
  
# Installing Transpect epubtools-frontend

These notes are for OSX users, but also apply generally to most operating systems.

Below will get you started with a command line eBook generation workflow using an XHTML/CSS file set using the free and open source software Transpect module *epubtools-frontend*. For full guidelines on the whole process, designing and editing your book see https://github.com/hybrid-publishing-group/book-coding

Thanks from - [Berlin.Publishing-School.net](http://berlin.publishing-school.net)

1. Create a GitHub account https://github.com/join
2. Download GitHub desktop app https://desktop.github.com/
3. Use your GitHub user account and log into the desktop app
4. Now add two repositories from GitHub to your GitHub desktop app
  * Transpect epubtools-frontend https://github.com/transpect/epubtools-frontend 
  
    Note: if your cloning via the terminal you need to use a recursive cloning `$ git clone git@github.com:transpect/epubtools-frontend.git --recursive` otherwise Transpect internals will be missing.
    
  * #psberlin book templates https://github.com/hybrid-publishing-group/book-coding 
5. Install Java™ Platform, Standard Edition Development Kit (SDK) 1.8+ - http://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.html
6. Launch your command line interface (CLI) AKA *terminal* from /applications/ultilities/terminal.app or by another method on Linux or Windows
7. In the terminal navigate to /Documents/Github/epubtools-frontend using `cd Documents/Github/epubtools-frontend` or to wherever you have your Github repositories stored. NB: Basic Mac command line cheat sheet https://gist.github.com/poopsplat/7195274
8. Now you can make eBooks by entering the following command in the terminal, the terminal output will give you the name and location of the outputted eBook file: 
```
$ ./epubconvert epubtools/samplexhtml/samplexhtml.xhtml
```
Terminal output
```
starting epubconvert
writing EPUB file => epubtools/samplexhtml/samplexhtml.epub
epubconvert finished, for details see epubtools/samplexhtml/samplexhtml.log
```
Voilà!

You can also use the #psberlin book template here to make an ebook, and edit and design the book as you like. Run the following command:
```
$ ./epubconvert ../book-coding/template2/template2.xhtml
```
Any questions ping us on Twitter [@hy_pub](https://twitter.com/@hy_pub) or log an issue on Github.

# Session #3 02.08.2017 - Responsive web, distribution, refresh

We'll start with building a sample book from some Mute Magazine Anthology content to test out Vivliostyle, Transpect and then distro the publications (eventually)!

## Responsive Web

 * Get Bootstrap - http://getbootstrap.com/getting-started/
 * Bootstrap tutorial - https://www.w3schools.com/bootstrap/default.asp
 
## Distribution

 * Pod, eBook. Ingram Spark or Lightning Source - http://www.ingramspark.com/ - https://myaccount.lightningsource.com/ or local supplier 
 * Kindle Direct - https://kdp.amazon.com
 * Google Books and Play, Amazon Look Inside, Archive.org
 * Amazon Seller Central
 * GitHub - and related, GitBooks Caliban and the Witch https://www.akpress.org/calibanandthewitch.html and https://www.gitbook.com/book/anarchivists/caliban/details
 * Lots of academic options with Open Access
 
 ## Refresh: Transpect, Vivliostyle, GitHub
 
 



 
 
