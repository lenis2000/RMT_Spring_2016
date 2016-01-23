## MATH 8380 Random Matrices
##### Spring 2016. Department of Mathematics, University of Virginia

## Notes on TeX style

1. Please do not define and use any \newcommand commands!

2. Try to be consistent --- use environments provided:
		
	\begin{theorem}\label{thm:example}
		A theorem.		
	\end{theorem}
	\begin{proof}[Idea of proof]
		And here is an equation:
		\begin{align*}
			a^2+b^2=c^2.
		\end{align*}
		This concludes the proof.
	\end{proof}	

The above code produces:


Use 

	\align 

or 

	\multline 

for displayed equations.

3. Full list of theorem environments defined:


	\newtheorem{proposition}{Proposition}[section]
	\newtheorem{lemma}[proposition]{Lemma}
	\newtheorem{corollary}[proposition]{Corollary}
	\newtheorem{theorem}[proposition]{Theorem}
	\newtheorem{definition}[proposition]{Definition}
	\newtheorem{remark}[proposition]{Remark}
	\newtheorem{example}[proposition]{Example}
	\newtheorem{exercise}[proposition]{Exercise}	


4. Use 
	
	\note 

command to insert notes: \note{this is a note}.

5. Use understandable labels for theorems and equations, and reference them by using 

	\ref

or 

	\eqref 

like this: \ref{thm:example}. Little hints for links will appear in the PDF file, this should help you.

6. Bibliography links can be inserted using the 

	\cite

command. I am using a single huge BiBTeX file which is at [https://github.com/lenis2000/BiBTeX/blob/master/bib.bib](https://github.com/lenis2000/BiBTeX/blob/master/bib.bib).
If something is not in that file, leave a note. 
Example: command 

	\cite{AndersonGuionnetZeitouniBook}

produces a citation to the book by Anderson, Guionnet, and Zeitouni.

7. You can email me your TeX files (in which case take
my preamble and put your text into it), or alternatively you can use GitHub's pull requests mechanism
[https://help.github.com/articles/using-pull-requests/](https://help.github.com/articles/using-pull-requests/).
