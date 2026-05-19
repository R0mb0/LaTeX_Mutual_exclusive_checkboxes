# LaTeX Mutual exclusive checkboxes

[![made-with-latex](https://img.shields.io/badge/Made%20with-LaTeX-1f425f.svg)](https://www.latex-project.org/)
[![Compilation_Test](https://github.com/R0mb0/LaTeX_Mutual_exclusive_checkboxes/actions/workflows/Compilation_Test.yml/badge.svg)](https://github.com/R0mb0/LaTeX_Mutual_exclusive_checkboxes/actions/workflows/Compilation_Test.yml)
[![pages-build-deployment](https://github.com/R0mb0/LaTeX_Mutual_exclusive_checkboxes/actions/workflows/pages/pages-build-deployment/badge.svg)](https://github.com/R0mb0/LaTeX_Mutual_exclusive_checkboxes/actions/workflows/pages/pages-build-deployment)
[![Codacy Badge](https://app.codacy.com/project/badge/Grade/22052986429e4b1fa202b97e9061589f)](https://app.codacy.com/gh/R0mb0/LaTeX_Mutual_exclusive_checkboxes/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade)

[![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://github.com/R0mb0/LaTeX_Mutual_exclusive_checkboxes)
[![Open Source Love svg3](https://badges.frapsoft.com/os/v3/open-source.svg?v=103)](https://github.com/R0mb0/LaTeX_Mutual_exclusive_checkboxes)
[![Donate](https://img.shields.io/badge/PayPal-Donate%20to%20Author-blue.svg)](http://paypal.me/R0mb0)

---

<div align="center">
  <a href="http://paypal.me/R0mb0">
    <picture>
      <source media="(prefers-color-scheme: dark)" srcset="https://github.com/R0mb0/Support_the_dev_badge/blob/main/Badge/SVG/Support_the_dev_badge_Dark.svg">
      <source media="(prefers-color-scheme: light)" srcset="https://github.com/R0mb0/Support_the_dev_badge/blob/main/Badge/SVG/Support_the_dev_badge_Light.svg">
      <img alt="Saved you time? Support the dev" src="https://github.com/R0mb0/Support_the_dev_badge/blob/main/Badge/SVG/Support_the_dev_badge_Default.svg">
    </picture>
  </a>
</div>


## Minimal working example

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

<a href="https://github.com/R0mb0/Not_made_by_AI">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://github.com/R0mb0/Not_made_by_AI/blob/main/Badge/SVG/NotMadeByAIDark.svg">
    <source media="(prefers-color-scheme: light)" srcset="https://github.com/R0mb0/Not_made_by_AI/blob/main/Badge/SVG/NotMadeByAILight.svg">
    <img alt="Not made by AI" src="https://github.com/R0mb0/Not_made_by_AI/blob/main/Badge/SVG/NotMadeByAIDefault.svg">
  </picture>
</a>
