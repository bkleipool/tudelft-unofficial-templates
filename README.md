# TUDelft Unofficial Templates
This repository contains unofficial TU Delft templates for reports, assignments and summaries. These templates were created from the need for professional-looking, reusable LaTeX templates without unnecessary clutter. The main benefit of these templates are that they render much faster than the official templates and they do not contain any code that the average LaTeX user wouldn't be familiar with (no .sty files or internal TeX commands), meaning that the average LaTeX user can easily troubleshoot any potential errors that might occur.

### Contents of this page
- [Templates](#templates)
    + [The Report template](#the-report-template)
    + [The Assignment template](#the-assignment-template)
    + [The Summary template](#the-summary-template)
- [Usage](#usage)


# Templates

### The Report template
The report template is intended to be used for large design reports (20+ pages). It contains a front page with room for up to 10 authors and a mentor, as well as the title and potential subtitle of the report. The template contains a list of figures (LoF), list of tables (LoT), list of symbols (LoS) and a bibliography in the AIAA style.

The `.tex` files for the chapters of the report are stored in the `chapters` folder. When chapters are renamed or new chapters are added, the `.tex` file should be (re)named accordingly. The `\chapter{}` command is placed in `main.tex`, *not* in the chapter file itself. Figures and tables are placed in the `Figures` folder. However, for a report with a large amount of tables a `Tables` folder may also be appropriate, since it is preferable to place the `\begin{tabular}...\end{tabular}` environment of large tables in a separate `.tex` file to prevent clutter. 

![](Report%20Template/report-preview.png)

### The Assignment template
The assignment template is intended to be used for smaller (individual) assignments (5-20 pages). The front matter is largely the same as the report template, except that it does not contain an LoF, LoT or LoS and the table of contents is listed on the front page.

Figures and tables are placed in the `Figures` folder. However, for an assignment with a large amount of tables a `Tables` folder may also be appropriate, since it is preferable to place the `\begin{tabular}...\end{tabular}` environment of large tables in a separate `.tex` file to prevent clutter. 

![](Assignment%20template/assignment-preview.png)

### The Summary template
The summary template is intended to be used for course summaries, but can also useful for taking lecture notes. The summary template offers special boxed environments, `\begin{FO}...\end{FO}` for Formulas and `\begin{WE}...\end{WE}` for Worked Examples (see the [example](Summary%20Template/Main.tex#L155)). Their respective primary and secondary colors can be changed in the [preamble](Summary%20Template/Main.tex#L12).

![](Summary%20Template/summary-preview.png)

# Usage
These templates can easily be imported into [Overleaf](https://www.overleaf.com/) by clicking `New Project`>`Upload Project` and uploading a `.zip` file listed in this repository.
