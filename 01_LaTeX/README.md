# LaTeX

LaTeX is used to prepare well-structured documents, especially when a report contains formulas, figures and references. Instead of setting everything manually, we write commands in a .tex file and compile it to get a document, usually a PDF. Overleaf is an online option, while TeXstudio with a TeX distribution can be used offline.

## Starting a document

The document class decides the general layout. Article is common for short reports, while report and book are better suited to longer work. A basic document begins with \documentclass{article}, followed by \begin{document} and \end{document}. Extra features are loaded using \usepackage{...} before the document starts.

Headings are made with \section{...} and \subsection{...}. A title can be created with \title{...}, \author{...}, \date{...} and \maketitle. Lists use itemize for bullet points and enumerate for numbered points. Commands such as \textbf{...}, \textit{...} and \underline{...} change the appearance of selected text.

## Mathematical content

LaTeX is particularly helpful for equations. Inline mathematics is written within dollar signs, and displayed mathematics can be written using the display-math delimiters. Common commands are \frac{a}{b} for fractions, \sqrt{a} for square roots, ^ for superscripts and _ for subscripts. Greek letters such as \alpha and \beta are written using their names. Equations can be aligned using appropriate mathematical environments; matrices can be created with matrix, pmatrix or bmatrix environments.

## Tables and pictures

The tabular environment arranges data into rows and columns. The & symbol separates columns and a double backslash ends a row. \hline draws a horizontal rule. Tables with headings and numbering can be placed inside the table environment with a caption and label. The multirow and multicolumn commands help when cells need to span rows or columns.

Images are generally inserted with the graphicx package and \includegraphics{...}. A figure environment can hold the image, caption and label. The picture environment is different: it can draw basic lines, arrows, boxes and circles using coordinates, \put, \line and \circle.

## Layout and references

The geometry package helps set margins. Page styles control headers, footers and page numbers; fancyhdr allows more customization. The xcolor package is used for coloured text. \tableofcontents can generate a contents list. With \label{...} and \ref{...}, figures, tables and sections can be referred to without typing their numbers manually. Bibliographies and citations help keep sources organized in larger reports.
