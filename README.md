A LaTeX template for a beamer of size 16:9. The template consist of a KU-folder with imagefiles, a picture-folder consisten of examples of imagefiles, a KUstyle.sty file and a main.tex file.

IMPORTANT! In order for the document to compile, one needs to use XeLaTeX or LuaLaTeX as compiler. This can be done in  Overleaf by Menu -> Settings -> Compiler -> Choose XeLaTeX/LuaLaTeX

To change the text at the top, then change the 'toplinje' command in the document-enviromnet.

The template consist of a frontpage and different examples of slides. At the frontpage one can for instance change the main title, subtitle and backgroundimage.

A new slide is added by using the frame-environment. It's important that either [hvid], [rod] or [billede] is include af \begin{frame}. [hvid] makes a white background, [rod] makes a red background and [billede] adds an image to the background. It you use [billede] it's important to change the \setbeamertemplate{background} command (an example is included in the main.tex file)

If one whises to print the beamer st. it exand to A4 size, one can add the following code before \begin{document}

\usepackage{pgfpages}
\pgfpagesuselayout{resize to}[a4paper,landscape,border shrink=5mm]