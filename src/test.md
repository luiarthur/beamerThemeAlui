---
bibliography: test.bib
bibliographystyle: plain 

header-includes:
    - \usepackage[T1]{fontenc}
    - \usepackage{amssymb,bm,mathtools,amsmath}
    - \usepackage{graphicx,caption,float}
    - \def\beginmyfig{\begin{figure}[ht]\begin{center}}
    - \def\endmyfig{\end{center}\end{figure}}
    - \def\ds{\displaystyle}
    - \newcommand{\tbf}[1]{\textbf{#1}}
    - \def\inv{^{\raisebox{.2ex}{$\scriptscriptstyle-1$}}}
    - \def\pm{^{\raisebox{.2ex}{$\scriptscriptstyle\prime$}}}
    - \newcommand{\norm}[1]{\left\lVert#1\right\rVert}
    - \newcommand{\p}[1]{\left(#1\right)}
    - \newcommand{\bk}[1]{\left[#1\right]}
    - \newcommand{\bc}[1]{ \left\{#1\right\} }
    - \newcommand{\abs}[1]{ \left|#1\right| }
    - \def\I{\bm I}
    - \def\N{\mathcal N}
    - \newcommand{\mat}{ \begin{pmatrix} }
    - \newcommand{\tam}{ \end{pmatrix} }
    - \newcommand{\m}[1]{\mathbf{\bm{#1}}} # Serif bold math
    # Title:
    - \title[IBP]{\textbf{Some Title}}
    - \author[Arthur Lui]{Arthur Lui}
    - \institute{ AMS\\ UC Santa Cruz \footnote{UCSC is awesome}}
    - \date{\today}
---

\titlepage

# Best equation ever
Hi there

$$\bm{y = X\beta + \epsilon}$$

$$
{\hat{\m\beta}} = (\m{X'X})^{-1}\m{X'}\m y
$$

# Yes
![Mondrian](mondrian.jpg)

# IBP

I just cited [@griffiths2011indian].
And now I'm citing @williamson2010dependent

# List

- item 1
- item 2
