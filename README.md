# LaTeX Report

* `View`: [main.pdf](https://github.com/rodrigowra/report/blob/master/main.pdf)

* `The report can be downloaded at` : <https://github.com/rodrigowra/report/archive/master.zip>

### Usage

```bash
pdflatex main.tex
bibtex main.tex
pdflatex main.tex
```

### Dependencies

```bash
sudo apt-get install texlive-full
```
main.tex
-----
<!---
Add the contents of `myfile.tex` into your LaTeX source code, for example using `\input{myfile.tex}`. 
Make sure that the required packages (such as `pgfplots`) are loaded in the preamble of your document as in the example:
-->
```latex
\documentclass[a4paper,11pt]{article}
\input{configs.tex}
\begin{document}
\input{title.tex}
\newpage
\tableofcontents
\thispagestyle{empty}
%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%
\newpage
\section{Introdução}
\section{Section 1}
\section{Section 2}
\section{Section 3}
\section{Conclusão}
\newpage
%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%
%to insert references
\nocite{ams} 
\addcontentsline{toc}{section}{Referências}
\renewcommand\refname{Referências}
%\bibliographystyle{abntex2-alf}
\bibliographystyle{plain}
\thispagestyle{empty}
\bibliography{referencias}
\thispagestyle{empty}
%\listoftodos
%Example text \todo{Mude aqui} and more text
%\listoftodos[List of suggested changes]
\end{document}
```
