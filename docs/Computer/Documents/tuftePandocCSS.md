```powershell
pandoc  --katex --section-divs --from markdown+tex_math_single_backslash --filter pandoc-sidenote --to html5+smart --template=tufte.html5 --css=.\tufte-css\tufte.css --css=.\pandoc.css --css=pandoc-solarized.css --css=.\tufte-extra.css -o $OUTPUT -s $SOURCE
```