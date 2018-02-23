# csm-thesis

## Caveat Emptor
This template is provided ﻿“AS IS” without warranty of any kind, either
expressed or implied, including, but not limited to, the implied warranties
of merchantability and fitness for a particular purpose.  The entire risk as
to the quality and performance of the template is with you.  Should the
template prove defective, you assume the cost of all necessary servicing,
repair or correction.

## ChangeLog

### 2018-02-23
  * Removed "empty section" requirement.

### 2017-10-12
  * Added compatibility with the "cleveref" package.
  * Added a "chapterbold" option that bolds all the chapter headings.
  * Fixed appendix behavior to match chapter behavior.
  * Fixed a small miscalculation in the placement of the page number on landscape pages.
  * Fixed a bug where sideways tables/figures in sequence could cause some pages to not be rotated.
  * Fixed a bug where multiple "List of Symbols" categories placed all symbols in the last category.
  * Changed Appendicies that appear within chapters to be subsections (for journal-type publications).
  * Changed the List of Abbreviations temporary filename so that it does not conflict with packages providing a List of Algorithms.

### 2012-12-11
  * Fixed some issues with landscape oriented pages.
  * Fixed a bug where the \vref command stopped working properly.
  * Changed the footnote settings to be flush with the left margin.
  * The "\degree" command is now deprecated, use "\degreetitle" instead.
  * The "nolabel" option now provides better behavior in the figure/table lists.
  * Fixed an issue where using the \tabular* environment resulted in a missing caption error.
  * Removed the "pocket" appendix/contents commands, as these entries are no longer permissible.
  * Fixed an issue where chapters in the appendix section do not appear as appendices under certain circumstances.
  * Added setting to losen formatting rules for existing journal articles: "\journalarticle" and "\endjournalarticle".
  * Added new commands to help with notating journal articles in a thesis: "\authornotesymbol" and "\authornotenumbered".
  * Added two special commands for handling sections for existing articles in a thesis: "\bumpsections" and "\unbumpsections".

### 2012-09-23
  * Added preliminary support for the new guidelines.
  * Changed the LyX example document encoding to UTF-8.
  * Added support for the "chapterbib" and "bibtopic" packages.
  * Changed the example table to use the default placement rules.
  * Added the ability to create "parts" as groupings around chapters.
  * Changed the "introduction" environment to be treated as a chapter.
  * Revised the equation that ensures a minimum of one "leader dot" before page numbers.
  * The list of tables and the list of figures now auto-calculate the "number" box size.
  * Fixed a rare issue where the "pocket" table of contents entries would not be displayed.
  * Combined lists are now ensured to have the same indent after the Figure/Table identifier.
  * The user may now set the bibliography style to something other than unsrtnat and authordate1.
  * Revised the equation that ensures sufficient space for the chapter/appendix numbers in the contents.
  * Equations that are followed by a paragraph starting with a lower-case letter are no-longer indented.
  * Fixed a bug where documents would not compile if the "pdfpages" package was included after the template.

### 2012-03-09
  * Single-spacing is now used by default within normal tables.
  * Preliminarily incorporated the documentation into the template.
  * Fixed an issue that caused extra space after "Here Definitely" floats.
  * The template now generates an error for unreferenced figures and tables.
  * Fixed a bug where the document would not compile if hyperref was disabled.
  * Fixed where headers did not appear on every page for portrait-mode longtables.
  * Added the ability to create sub-lists for the "List of Symbols"/"Nomenclature" list.
  * The template now automatically adds the "Continued." caption for multi-page longtables.
  * Changed an instance of "\nobreakdash" (requires amsmath) to "\nobreakdashes" (normal LaTeX).
  * Wrapping a figure or table in the "landscape" environment will no-longer force a page break.
  * Added an optional "\ShowSymbolFirst" command for the "List of Symbols" (nomenclature) items.
  * Fixed a bug where the space before an in-line figure or table did not exactly match the space afterward.
  * The spacing between tables and their captions is now correct when the "center" environment is used instead of "\centering".

### 2011-09-07
  * Multi-line headings are now single-spaced.
  * Added support for "\paragraph" (3rd tier section).
  * Fixed weirdness with dashes in the "List of Abbreviations".
  * Fixed where some list entries could over-flow the size box.
  * Changed default (document recommended) print scaling to "None".
  * The "math mode" font will now automatically be set to the document font.
  * Chapter headings are now appropriately one line down from the top margin.
  * Fixed a spurious space between "et al." and the comma in author-date references.
  * Fixed a bug where the space before an equation did not match the space afterward.
  * Fixed a problem where in some circumstances footnotes were not flush with the bottom margin.
  * Orphaned lines (a single line of a paragraph at the end of a page) can no-longer be generated.
  * Fixed a bug where captions did not display any reference labels when "nolabel" mode is enabled.
  * Added preliminary support for automatic equation breaking (add "\usepackage{breqn}" to the LaTeX Preamble to enable).
  * Fixed a bug where a large number of floats on the first page of a chapter could cause the "too many unprocessed floats" error.
  * Fixed a bug in the table handling that could cause the free float list to become corrupted ("too many unprocessed floats" error).

### 2011-06-01
  * Fixed a mysterious compile issue with LyX 2.0.
  * Revised how blank pages are handled by hyperref.
  * Added line numbers to several of the error messages.
  * Fixed using "\includegraphics" outside of figure floats.
  * LyX now displays more accurate figure and table numbering.
  * The thesis title now vertically centers absolutely perfectly.
  * Added "\addpocketappendix" to simplify adding external appendices.
  * Fixed where the new rotation support did not enable properly in LyX.
  * Changed spelling of "acknowledgments" to the more widely used version.
  * Added "here if possible" to the default permitted float placement list.
  * Fixed a bug where equations were not properly labeled in the appendices.
  * Fixed a bug where references would sometimes split across a page boundary.
  * Paragraphs following "itemize" and "enumerate" environments are now indented.
  * Fixed a minor float placement bug when using "\csmfigure" or "\csmlongfigure".
  * Fixed a bug where automatically renaming the appendix did not always work properly.
  * Changed the appendix detection behavior to no-longer require an additional temp file.
  * Fixed indentation for multi-line chapter and appendix titles in the Table of Contents.
  * List entries can no-longer fill all the way to the page number without placing a fill dot.
  * Changed default float behavior to not place floats on the top of the first page of a chapter.
  * Fixed a bug where "author-date" references were not indented after the first line of a reference.
  * Documents will no-longer compile if a "Here Definitely" float splits the text across a page boundary.
  * Added support for LyX's built-in appendix feature (better in-editor section, figure, and table numbering).
  * Disabled "in-viewer" page rotation for sideways figures and tables (due to a currently unresolved figure placement bug).

### 2011-04-07
  * Added support for the "landscape" environment.
  * Added support for the "sidewaysfigure" and "sidewaystable" environments.
  * Added an example of using the "longtable" environment for multi-page tables.
  * Fixed a bug where some multi-line equations were being double-spaced incorrectly.
  * Fixed a bug in LyX where hyperref page titles included garbage unicode characters.
  * Fixed a bug where cross-referencing an appendix did not use the correct numbering.
  * Fixed a bug where a warning for the references section was printed in the document.
  * Fixed a bug where including a float "Here Definitely" would break the 20th float later.
  * When using two-sided documents (and hyperref) printing is now set to default to duplexing.
  * Added autosort ability for "\listofsymbols" and "\listofabbreviations", see example document.
  * Fixed a bug where a significant amount of extra space would appear before equations for LyX users.
  * Fixed a bug in the LyX layout where the "setspace" package was being included after hyperref (install new LyX layout!).
  * The "\listoffiguresandtables" command now automatically outputs two separate lists when there's more than two items in either list.

### 2011-02-28
  * Added support for including hyperref before the template.
  * Made including citations in captions no-longer require special code.
  * LyX no-longer requires anything in the preamble to produce a document.
  * Changed the inclusion of hyperref to use the standard \usepackage command.
  * Added an example of a child document in both the LaTeX and LyX example files.
  * Added an example of a "table of figures" shortened caption for the LyX example document.
  * When using natbib, the appropriate numerical/author-date style is now automatically included.
  * Added the "url" package to the template requirements so citations with URLs do not produce an error.
  * Changed the LyX examples for adding symbols/nomenclature/abbreviations to permit easier copying and pasting.

### 2011-02-03
  * Fixed some bugs in the LyX installation script.

### 2011-02-02
  * Fixed a mistake where the signature date blocks were not double-spaced.
  * Changed the BibTeX style in the LyX example to use "unsrtnat" by default.
  * Updated the template for the new caption placement guidelines (not yet posted).
  * Integrated natbib better with LyX (sort&compress is now automatically activated).
  * Added support for using the built-in LyX features for adding "List of Symbols" (nomenclature) items.

### 2010-08-18
  * Added the ability to redefine the figure/table labels.
  * Fixed a bug where the "\atom" command only worked with hyperref enabled.
  * Added support for using the "listings" package without generating warnings.
  * Added additional styles to the LyX layout to reduce the amount of direct LaTeX calls.
  * Hyperref cross-references to figures now go to the top of the figure instead of the caption.
  * Fixed a bug where optional parameters were not allowed for the "biblatex" package's "\printbibliography" command.
  * Upgraded to using the newer "subfig" package instead of "subfigure" for multiple-figure floats, please note that if you are upgrading an old document you may need to remove \usepackage{subfigure} from your document preamble.

### 2010-05-15
  * Added a "dedication" environment for inserting a dedication page.
  * Added a "\listofabbreviations" example to the LyX version of the template.
  * Fixed a compatibility issue when used in conjunction with the "biblatex" package.
  * Fixed hyperref bookmarks to reference before the title of a section instead of afterward.
  * Fixed a bug in "insane" mode where pages are not properly renumbered if no "\makesubmittal" call exists.
  * Added an optional parameter for the "\listofsymbols" command to re-title the section (ie. "\listofsymbols[Nomenclature]").

### 2010-04-12
  * The template now generates an error when a section is empty.
  * Fixed a bug with double-spacing references when using the "natbib" package.
  * Single-sided documents no-longer generate a blank page before new chapters.
  * The "\newoddpage" command is now replaced with the standard "\cleardoublepage" command.
  * Fixed handling of LaTeX commands in the title when "automatic title triangulation" is enabled.
  * Using "manual title triangulation" with hyperref no-longer results in character encoding warnings.
  * Fixed a bug where figures and tables just before the references could float to the references page.
  * The standard "\cleardoublepage" command is now redefined to create a blank page with no page number.
  * To retain compatibility with older documents, the "\newoddpage" is now an alias for "\cleardoublepage".
  * Added an "\atom{mass number}{proton number}{symbol}{ionization}{# atoms}" convenience command for using chemical symbols in the title and chapter commands.

### 2010-04-06
  * Added a "\makecopyright{year}" convenience command.
  * Fixed some incompatibilities with the "natbib" package.
  * Fixed the page numbering when there is a copyright page.
  * The "natbib" package is now used by default (in the example) for citations.

### 2010-03-23
  * Added an "insane" option to disable the document format review checks (for rendering sub-documents).
  * Added a "nolabel" option to turn off the automatic addition of "Figure~" and "Table~" to figure and table references.  Please note that your caption reference must match your document reference to comply with OGS guidelines.

### 2010-02-12
  * Added preliminary support for the biblatex package.
  * Fixed long lists (toc, lof, etc.) when using the hyperref package.
  * Captions inside a "subfigure" are now automatically single-spaced.
  * Fixed a bug where "\cite" in a figure caption would not allow the document to compile.
  * Fixed some compatibility issues with hyperref where references were not correct internally.
  * The convenience functions "\csmfigure" and "\csmlongfigure" are no-longer included "here" [H] by default.
  * If exactly one appendix is included then the appendix label (A) is now removed.  Depending on your software package you may need to manually re-compile your document (Kile will re-run automatically, WinEdit will not).

### 2009-11-03
  * Added "\listofabbreviations" capability, add an abbreviation with \addabbreviation{<explanation>}{<abbreviation>}.
  * Fixed a bug where referencing a subfigure generated an incorrect reference.
  * Fixed a bug where creating an inverted pyramid title manually was disabled.
  * Fixed some minor alignment issues with automatic pyramid titles.
  * Fixed compatibility issues with the "hyperref" package.

### 2009-10-21
  * Added "\listofsymbols" capability, add a symbol with \addsymbol{<explanation>}{$<symbol>$}.
  * The automatic inverted pyramid title should now work properly under most circumstances.
  * Fixed a bug in the detection of whether the list of tables and/or figures is required.
  * Fixed a bug where the "acknowledgements" section was being required.
  * The greater than (>) and less than (<) symbols now encode as text.

### 2009-07-08
  * Now warns the user if the abstract is longer than 350 words (the limit for a PhD thesis).
  * Added preliminary support for one sided pages.
  * No-longer conflicts with the "color" package.

### 2009-05-09
  * Now includes preliminary support for automatically creating the inverted pyramid title.
  * Now stops the user from including the "fullpage" package (messes with the margins).

### 2009-04-27
  * Fixed a bug where "List of Tables and Figures" is displayed when there are no tables.
  * Using "subfigure" no-longer adds blank entries to the list of tables and figures.

### 2009-04-01
  * List of Figures/Tables and References Cited now single-space multi-line entries.

### 2009-03-26
  * Removed error when "\listoffigures" and "\listoftables" are used individually rather than using "\listoffiguresandtables."
  * Fixed equation numbering not restarting after each new chapter.

### 2009-03-25
  * Added additional space between Figure and Table labels and the description in the Table of Contents.
  * Fixed Figure and Table labels in Appendices to use the correct Appendix value (ie. Figure~A.1).
  * Simplified single-siding the front matter so that "\newpage" no-longer needs to be redefined.
  * Added additional styles to the LyX layout to reduce the amount of direct LaTeX calls.

### 2009-03-09
  * Correctly redefines the label created using the "\label" command for every new "section" (all chapters and subsections).
  * Automatically titles the "List of Tables and Figures" appropriately if one or the other does not exist.
  * Warns about having a "List of Tables and Figures" section if there are no tables AND no figures.
  * There is a new "\newappendixnum" and "\appendixnum" command for adding "pocket" appendices.
  * Properly single-sides the front matter when any of the sections is longer than a page.
  * Detects missing sections and generates an error forcing you to fix the problem.
  * There is a new "\appendix{<Title of Appendix>}" command for appendices.
  * Now includes examples of inserting figures and tables.

### 2009-03-05
  * Redefines the "\newpage" command properly instead of using a special "\nextpage" command.
  * Detects errors such as missing "\author", "\title", "\degree", "\advisor", etc.
  * Includes a LyX "layout" file to make it easy to work directly in LyX.
  * Uses a special environment for each of the necessary components.

### 2009-03-04
  * Properly automatically capitalizes the title even if there are carriage returns in it.
  * Fixed an incompatibility between the "\chapter" command and AMS-LaTeX.

### 2009-03-03
  * The co-advisor (\coadvisor{<name>}) is now optional (the signature page reflects this properly).

### 2009-02-04
  * First public release.
