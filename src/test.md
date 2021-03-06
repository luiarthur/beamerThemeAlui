---
# COMMENT OUT IF NOT USING BIBLIOGRAPHY
bibliography: test.bib  
bibliographystyle: plain
# This is how you use bibtex refs: @nameOfRef
# see: http://www.mdlerch.com/tutorial-for-pandoc-citations-markdown-to-latex.html

header-includes:
    - \usepackage[T1]{fontenc}
    - \usepackage{amssymb,bm,mathtools,amsmath,bbm}
    - \usepackage{graphicx,caption,float}
    - \def\beginmyfig{\begin{figure}[H]\begin{center}}
    - \def\endmyfig{\end{center}\end{figure}}
    - \newcommand{\tbf}[1]{\textbf{#1}}
    # MATH
    - \def\inv{^{\raisebox{.2ex}{$\scriptscriptstyle-1$}}}
    - \newcommand{\m}[1]{\mathbf{\bm{#1}}} # Serif bold math
    - \newcommand{\norm}[1]{\left\lVert#1\right\rVert}
    - \newcommand{\p}[1]{\left(#1\right)}
    - \newcommand{\bk}[1]{\left[#1\right]}
    - \newcommand{\bc}[1]{ \left\{#1\right\} }
    - \newcommand{\abs}[1]{ \left|#1\right| }
    - \newcommand{\mat}{ \begin{pmatrix} }
    - \newcommand{\tam}{ \end{pmatrix} }
    - \newcommand{\suml}{ \sum_{i=1}^n }
    - \newcommand{\prodl}{ \prod_{i=1}^n }
    - \newcommand{\ds}{ \displaystyle }
    - \newcommand{\df}[2]{ \frac{d#1}{d#2} }
    - \newcommand{\ddf}[2]{ \frac{d^2#1}{d{#2}^2} }
    - \newcommand{\pd}[2]{ \frac{\partial#1}{\partial#2} }
    - \newcommand{\pdd}[2]{\frac{\partial^2#1}{\partial{#2}^2} }
    - \newcommand{\N}{ \mathcal{N} }
    - \newcommand{\E}{ \text{E} }
    - \def\given{~\bigg|~}
    # Title:
    - \title[Short Title]{\textbf{Some Very Long and Fancy Title}}
    - \author[A. Lui]{Arthur Lui}
    - \institute{ AMS\\ UC Santa Cruz \footnote{UCSC is awesome}}
    # OTHER defs:
---

[//]: # (Make Title Page)
\date{\today}
\titlepage


# Math Slide

Some text.

$$
\bm{y = X\beta + \epsilon}
$$

$$
{\hat{\m\beta}} = (\m{X'X})^{-1}\m{X'}\m y
$$


# Inserting an image
![Mondrian](mondrian.jpg)

# Inserting several image
\beginmyfig
![Mondrian](mondrian.jpg){ height=20% }
![Mondrian](mondrian.jpg){ height=20% }
![Mondrian](mondrian.jpg){ height=20% }
![Mondrian](mondrian.jpg){ height=20% }  
![Mondrian](mondrian.jpg){ height=20% }
![Mondrian](mondrian.jpg){ height=20% }
![Mondrian](mondrian.jpg){ height=20% }
![Mondrian](mondrian.jpg){ height=20% }
\caption{Eight Mondrians}
\endmyfig


# Resize Image
Here is text.
\beginmyfig
\includegraphics[height=0.5\textwidth]{mondrian.jpg}
\caption{This is a caption.}
\endmyfig


# Citations

I just cited [@griffiths2011indian].
And now I'm citing @williamson2010dependent
Citation Teh [-@teh2007stick].

# List

- item 1
- item 2
    1. Apple
    2. Orange
        1. Cat
        2. Dog
