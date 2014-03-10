MySlides
========

LaTeX Slides styles using tikz


# Example:

\documentclass{ryslidepyramid}
\usepackage{fancyvrb}
\renewcommand{\theFancyVerbLine}{%
   \color{gray!30}{\tiny\arabic{FancyVerbLine}}}
\title{暴风雨就要来了}
\author{Rainy}
\date{\today}
\begin{document}
\myfrontcover
\tableofcontents\thispagestyle{empty}
\newpage\section{星战前传}
\begin{itemize}
    \item 用 \LaTeX{} 制作幻灯片的宏包已有很多
    \item 自己比较习惯使用 \textsc{Beamer}
    \item 看了 ConTeXt 幻灯片设计
    \item 想用 \LaTeX{} 标准类文档制作几个类似风格
    \item 试试看
\end{itemize}
\newpage\section{取材和配方}
\begin{description}
    \item[geometry] 用于定制页面大小和布局
    \item[fancyhdr] 用于定制 header 和 footer
    \item[titling] 用于定制 title 样式等
    \item[ctex] 用于设置中文
    \item[tikz] 用于图形设计
    \item[eso-pic] 用于 {\sc Background} 设置
\end{description}
\newpage\section{使用方法简介}
\begin{itemize}
    \item 可以用{ \tt section} 作为 Slide 的标题
    \item 同时用{ \tt newpage} 制作下一张 Slide
    \item 其它的完全和用 \LaTeX{} 一样
    \item 没有{ \textsc{Beamer}} 那样的诸如{ \tt pause} 等一切效果
    \item 但是省去了写{ \verb"\frame"} 和{ \verb"\frametitle"} 的麻烦
\end{itemize}
\newpage\section{本文的{ \tt tex }源文件}
\fvset{fontsize=\scriptsize,numbers=left,numbersep=3pt}
\VerbatimInput{ryslide-test.tex}
\newpage\section{{\tt ryslide.cls} 文件}
\fvset{fontsize=\scriptsize,numbers=left,numbersep=3pt}
\VerbatimInput{ryslide.cls}
\newpage\section{Wiki 百科关于 \LaTeX{} 的简介}
\LaTeX{}（音译“拉泰赫”）是一种基于 \TeX{} 的排版系统，
由美国电脑学家莱斯利·兰伯特（Leslie Lamport）
在 20 世纪 80 年代初期开发，利用这种格式，
即使使用者没有排版和程序设计的知识也可以充分发挥由 \TeX{} 所提供的强大功能，
能在几天，甚至几小时内生成很多具有书籍质量的印刷品。
对于生成复杂表格和数学公式，这一点表现得尤为突出。
因此它非常适用于生成高印刷质量的科技和数学类文档。
这个系统同样适用于生成从简单的信件到完整书籍的所有其他种类的文档。
使用 \TeX{} 作为它的格式化引擎，当前的版本是 \LaTeXe{}。
\newpage
\vspace*{\fill}
{\centering\kaishu\color{white} 见\,\,\,好\,\,\,就\,\,\,收\\}
\vspace*{\fill}
\end{document}

