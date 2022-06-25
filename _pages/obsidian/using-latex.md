---
title: "LATEX Functions I Frequently Use"
categories:
  - Obsidian
  - LATEX
permalink: "/notes/obsidian/frequently-used-latex-function/"
---

- ## Functions I Frequently Use
	- ### Fraction
		- `g(x) &= \frac{1}{x}`
			- $g(x) = \frac{1}{x}$
	- ### Multiplication
		- not write a multiplication-sign at all, as in $y=mx+c$
		- or you should write it using a vertically centered dot, as in $3\cdot5=15$. Do **not** use symbols like "`*`"! In LaTeX you use the command `\cdot` to make a multiplication-dot.
		- Sometimes you can use the symbol $\times$. Code `\times` is used in LaTeX to make the symbol
	- ### Dynamic Bracket Size
		- The size of brackets and parentheses can be manually set, or they can be resized dynamically in your document, as shown in the next example:
		- `$F = G \left( \frac{m_1 m_2}{r^2} \right)$` will produce the following output: $F = G \left( \frac{m_1 m_2}{r^2} \right)$
		- Notice that to insert the parentheses or brackets, the `\left` and `\right` commands are used. Even if you are using only one bracket, _both_ commands are mandatory. `\left` and `\right` can dynamically adjust the size, as shown by the next example:
	- ### Formula steps
		- use this template to get the step calculation similar to example below
			```latex
			$$
			\begin{align*}
				Ent\\
					&= CR + PO \\ &= CR + (R-C_{roy}-CR)\cdot70\% \\
				\text{if C below cost ceiling} \\
					&= C + (R-C_{roy}-C)\cdot70\% \\
					&= 0.7R - 0.7C_{roy} + 0.3C
			\end{align*}
			$$
			```
		- ![[2022-04-20#^a2036b]]

---
## References
- [Learn LaTeX in 30 minutes - Overleaf, Online LaTeX Editor](https://www.overleaf.com/learn/latex/Learn_LaTeX_in_30_minutes#Adding_math_to_LaTeX)
	- [Documentation - Overleaf, Online LaTeX Editor](https://www.overleaf.com/learn)
- [LaTeX math and equations - LaTeX-Tutorial.com](https://latex-tutorial.com/tutorials/amsmath/)
- [LaTeX - Basic Code (malinc.se)](https://www.malinc.se/math/latex/basiccodeen.php#:~:text=In%20LaTeX%20you%20use%20the%20command%20cdot%20to,used%20in%20LaTeX%20to%20make%20the%20symbol%20%C3%97.)
