# Refactoring References
Documenting (and plotting) the most referenced refactorings from [Refactoring 2nd Edition](http://www.informit.com/store/refactoring-improving-the-design-of-existing-code-9780134757711).


## Rough "Algorithm"
- used pdf.js to read the file into memory
- save down the pdf to a text file
- read the text file into memory with node.js
- create a data structure based on the first page of Refactoring (note in the hardcover version of the book, all refactorings are listed with their corresponding page number).
  - Note,I saved this down as a json file.
- use regex to find the references (based on the json file described above)
- save the references as a data file
- use chart.js to plot the data

## Assumptions
- you have the refactoring 2nd edition pdf (note: this file is _not_ committed)
