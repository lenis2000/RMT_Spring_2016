## MATH 8380 Random Matrices
##### Spring 2016. Department of Mathematics, University of Virginia

## Notes on TeX style

<code>1.</code> Please do not define any new <code>\newcommand</code> commands! Here are some commands I am using, please try to use them, too:
	
	\newcommand{\SC}{\mathsf{SC}}
	
	\DeclareMathOperator{\EE}{\mathbb{E}}
	
	\DeclareMathOperator{\PP}{\mathbb{P}}

<code>2.</code> Try to be consistent --- use environments provided:
		
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

<img src=https://github.com/lenis2000/RMT_Spring_2016/blob/master/img/notes_tex_1.png>

Use 

	\align 

or 

	\multline 

for displayed equations.

<code>3.</code> Full list of theorem environments defined:

	\newtheorem{proposition}{Proposition}[section]
	\newtheorem{lemma}[proposition]{Lemma}
	\newtheorem{corollary}[proposition]{Corollary}
	\newtheorem{theorem}[proposition]{Theorem}
	\newtheorem{definition}[proposition]{Definition}
	\newtheorem{remark}[proposition]{Remark}
	\newtheorem{example}[proposition]{Example}
	\newtheorem{exercise}[proposition]{Exercise}	


<code>4.</code> Use 
	
	\note 

command to insert notes: <code>\note{this is a note}</code>.

<code>5.</code> Use understandable labels for theorems and equations, and reference them by using 

	\ref

or 

	\eqref 

like this: <code>\ref{thm:example}</code>. Little hints for links will appear in the PDF file, this should help you.

<code>6.</code> Bibliography links can be inserted using the 

	\cite

command. I am using a single huge BiBTeX file which is at [https://github.com/lenis2000/BiBTeX/blob/master/bib.bib](https://github.com/lenis2000/BiBTeX/blob/master/bib.bib).
If something is not in that file, leave a note. 
Example: command 

	\cite{AndersonGuionnetZeitouniBook}

produces a citation to the book by Anderson, Guionnet, and Zeitouni.

<code>7.</code> You can email me your TeX files (in which case take
my preamble and put your text into it), or alternatively you can use GitHub's pull requests mechanism
[https://help.github.com/articles/using-pull-requests/](https://help.github.com/articles/using-pull-requests/).
