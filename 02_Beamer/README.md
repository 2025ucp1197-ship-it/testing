# Beamer

Beamer is a LaTeX document class made for presentations. Instead of pages in a report, a Beamer document contains frames, which appear as slides. This is useful for technical presentations because headings, lists and mathematical formulas follow consistent formatting.

## Making slides

A presentation starts with \documentclass{beamer}. The main content is placed between \begin{document} and \end{document}. Each slide is written using \begin{frame}{Slide Title} and \end{frame}. The title inside the frame command appears as the slide heading.

To write points on a slide, the itemize environment is used for bullets and \item starts each point. The same idea works with enumerate when numbered steps are needed. A short presentation could have one frame for the introduction, another for key points and another for an example.

## Presentation features

Beamer supports overlays, so parts of a slide can appear in stages. It also provides slide layouts and presentation styling. Equations and other familiar LaTeX commands can be used inside frames, which is helpful for explaining technical subjects.
