# Refactoring References
Documenting (and plotting) the most referenced refactorings from [Refactoring 2nd Edition](http://www.informit.com/store/refactoring-improving-the-design-of-existing-code-9780134757711).


## Rough "Algorithm"
- use pdf.js to read the file into memory
- save down the pdf to a text file
- read the text file into memory with node.js
- create a data structure based on the first page of Refactoring (note in the hardcover version of the book, all refactorings are listed with their corresponding page number).
  - Note,I saved this down as a json file.
- use regex to find the references (based on the json file described above)
- save the references as a data file
- use chart.js to plot the data

## Development Phases
This project originally started off as three separate smaller projects:
- pdf (covert the refactoring pdf to text)
- regex (find all the refactoring references in the text file)
- charts (plot the references)

So...our phases

Phase 1 - `v0.0.1` (current)
- the above, i.e. "just get it working" :muscle:

Phase 2 - `v0.1.0` :bar_chart:
- integrate data with charts
- make charts dynamic (e.g. show "top 5" or "all" programmatically)
- move node_modules, project to top level

Phase 3 - `v1.0.0` :trophy:
- remove manual steps
- run entire project from one line

Phase 4 - `v2.0.0` :man_shrugging:
- TBD

## Immediate next steps
- make charts dynamic, currently the data was manually copy/pasted (:disappointed:)
- code cleanup, remove commented out code, etc. 

## Assumptions
- you have the refactoring 2nd edition pdf (note: this file is _not_ committed)
