# Large Latex Document Template

Can compile main for all sections or a single section at a time.

Note that LaTeX workshops PDF viewer can't find the section files. 

use the following settings:
```
    "latex-workshop.latex.outDir": "./out/",
    "latex-workshop.latex.tools": [
        {
            "name": "latexmk",
            "command": "latexmk",
            "args": [
                "-shell-escape",
                "-synctex=1",
                "-interaction=nonstopmode",
                "-file-line-error",
                "-pdf",
                "-aux-directory=./build/",
                "-outdir=./out/",
                "%DOC%"
            ],
            "env": {}
        },
```
