Move to `paper_w_supplement` direcotry.

To redirect the auxilliary files to the `out` directory, run with
```bash
pdflatex  -output-directory=out cicero
pdflatex  -output-directory=out supplement
bibtex out/cicero
bibtex out/supplement
pdflatex  -output-directory=out  cicero
pdflatex  -output-directory=out supplement
pdflatex  -output-directory=out  cicero
pdflatex  -output-directory=out supplement

```
The `pdflatex` steps need to be repeated thrice  to compile the figure and biblography references correctly. Not that the final pdf files will also be placed in the `out` directory.


