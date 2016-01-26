# AMIA LaTeX paper template

A basic AMIA (American Medical Informatics Association) style compliant LaTeX paper skeleton.

**Problem:** AMIA conference doesn't provide a LaTeX template for submissions. It only provides a Microsoft Word template. And we know the possible and unexpected problems of collaborating with Word.

**Solution:** Use pandoc to generate a skeleton from the Word template. Then, adapt the LaTeX file skeleton to make it look *as similar as possible* to the normal PDF output of Word.

## Compile

The file `amia-paper.tex` can be compiled using pdflatex or latex. However, these two compiler do not compile an output as the one required because they don't use Time News Roman font. LuaLaTeX or XeLaTeX compilers can be used instead. ([Texmaker] provides all the previous options.)

To compile the project using LuaLaTeX:
```bash
$ lualatex amia-paper.tex
$ bibtex amia-paper
$ lualatex amia-paper.tex
$ lualatex amia-paper.tex
```

## Bibliography

According to the recommended bibliography styles, I could find that `vancouver` is one of the most populars, and widely used in previous AMIA publications. If you have other suggestion, let me know.

[Texmaker]: http://www.xm1math.net/texmaker/

## License

[The MIT License (MIT)]((http://opensource.org/licenses/MIT))

Copyright (c) 2016 Emir Muñoz

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
