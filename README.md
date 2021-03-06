# Nek5000 Documentation

This is the repository of the [Nek5000](http://nek5000.mcs.anl.gov/) documentation 
written in LaTeX.

## How to build

* 'make' builds the user documentation in both PDF and HTML formats, as
  described below.  A subdirectory (build) is created for the output.

* 'make pdf' builds the user documentation in PDF format.  The PDF is a single
  file in the build directory (build/Nek_users.pdf).

* 'make html' builds the user documentation as a set of interlinked HTML 
  and image files.  The top-level table-of-contents is build/Nek_users.html.
  Supporting HTML and image files are also in the build directory.

## How to contribute

Please create a fork of the repository and make pull/merge requests. Keep in 
mind that the number of binary files should be kept minimal. The Makefile should be 
adapted to any special build requirements.

New issues or requests are welcome to be reported.

## How to publish on GitHub Pages

The Makefile target 'make gh-pages' will build and publish the HTML on the
[NekDoc GitHub Page][gh-page].  

To update the GitHub Page, a contributor must have write permissions to the main [NekDoc][main-repo] repository.  
The GitHub Page should *not* contain any edits that are newer than the [master branch][master] 
of the main repository.  Thus it is highly recommended to update the main repository
(through a merge/pull request, see ['How to contribute'](#how-to-contribute)) 
before publishing to the GitHub Page.

In summary, contributors who wish to update the GitHub Page should follow this workflow:

1. Create a fork of the repository
2. Edit the 'master' branch
3. Open a pull request
4. Publish to GitHub pages *after* the pull request has been merged

[gh-page]:   https://nek5000.github.io/NekDoc/Nek_users.html "Nek5000 user documentation on GitHub Pages"
[main-repo]: https://github.com/Nek5000/NekDoc "NekDoc repository"
[master]:    https://github.com/Nek5000/NekDoc/tree/master "NekDoc master branch"
