# LaTeX Mutual exclusive checkboxes

## Minimal example

```tex
\documentclass{article}
\usepackage{ocgx2}
\usepackage{tabularx}
\usepackage{amssymb}

\begin{document}
  \begin{tabularx}{\textwidth}{XX}
    {
      % First checkbox
			\begin{center}
				\leavevmode
				% Empty check
				\hbox{%
					\makebox[0pt][l]{%
						\begin{ocg}{Empty_check}{E}{1}%
							\Huge\actionsocg{ }{C, E1}{E, C1}{$\square$}%
						\end{ocg}%
					}%
				}%
				% Crossed check
				\hbox{%
					\makebox[0pt][l]{%
						\begin{ocg}{Crossed_check}{C}{0}%
							\Huge\actionsocg{ }{E}{C}{$\boxtimes$}%
						\end{ocg}%
					}%
				}%
			\end{center}
    }&{
      % Second checkbox
			\begin{center}
				\leavevmode
				% Empty check
				\hbox{%
					\makebox[0pt][l]{%
						\begin{ocg}{Empty_check}{E1}{1}%
							\Huge\actionsocg{}{C1, E}{E1, C}{$\square$}%
						\end{ocg}%
					}%
				}%
				% Crossed check
				\hbox{%
					\makebox[0pt][l]{%
						\begin{ocg}{Crossed_check}{C1}{0}%
							\Huge\actionsocg{}{E1}{C1}{$\boxtimes$}%
						\end{ocg}%
					}%
				}%
			\end{center}
    }
  \end{tabularx}
\end{document}
```


<details>
<summary>

## 👉 Click here to look the complete example! 👈

</summary>

[![Example](https://github.com/R0mb0/LaTeX_Mutual_exclusive_checkboxes/blob/main/Readme_imgs/document.png?raw=true)](https://github.com/R0mb0/LaTeX_Mutual_exclusive_checkboxes/tree/main/Example)

</details>
