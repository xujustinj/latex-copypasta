$$
% GENERAL UTILITIES
\newcommand{\defeq}{\mathrel{\mathop:}=}

% Parentheses and stuff
\newcommand{\pr}[1]{\left( #1 \right)}
\newcommand{\par}[1]{\mathopen{}\left( #1 \right)\mathclose{}}
\newcommand{\floor}[1]{\left\lfloor #1 \right\rfloor}
\newcommand{\ceil}[1]{\left\lceil #1 \right\rceil}
\newcommand{\size}[1]{\left| #1 \right|}
\newcommand{\norm}[1]{\left\lVert #1 \right\rVert}
\newcommand{\set}[1]{\left\lbrace #1 \right\rbrace}
\newcommand{\where}{\ \middle|\ }

% Functions
\newcommand{\func}[2]{\operatorname{#1}\,#2}
\newcommand{\parfunc}[2]{\operatorname{#1}\par{#2}}

% Cases
\newcommand{\if}[1]{\text{if \(#1\)}}
\newcommand{\ow}{\text{otherwise}}

% Left scripts
\newcommand{\lsub}[2]{{\vphantom{#1}}_{#2}#1}
\newcommand{\lsup}[2]{{\vphantom{#1}}^{#2}#1}
\newcommand{\lsubp}[2]{{\vphantom{#1}}_{#2}^{#3}#1}


% LINEAR ALGEBRA

\newcommand{\Span}[1]{\func{Span}{#1}}
\newcommand{\rank}[1]{\parfunc{rank}{#1}}
\newcommand{\dim}[1]{\parfunc{dim}{#1}}

% Matrices
\newcommand{\mat}[1]{{\begin{bmatrix} #1 \end{bmatrix}}}
\newcommand{\diag}[1]{\parfunc{diag}{#1}}

% Matrix functions
\newcommand{\tr}[1]{\parfunc{tr}{#1}}
\newcommand{\inv}{^{-1}}
\newcommand{\trans}{^T}

% Matrix subspaces
\newcommand{\Col}[1]{\parfunc{Col}{#1}}
\newcommand{\Row}[1]{\parfunc{Row}{#1}}
\newcommand{\Null}[1]{\parfunc{Null}{#1}}

% Linear mappings
\newcommand{\Range}[1]{\parfunc{Range}{#1}}
\newcommand{\Ker}[1]{\parfunc{Ker}{#1}}
\newcommand{\nullity}[1]{\parfunc{nullity}{#1}}

% Matrices of linear mappings
\newcommand{\coords}[2]{\mat{#1}_{#2}}
\newcommand{\cob}[3]{\lsub{\mat{#2}}{#1}_{#3}}
\newcommand{\coc}[2]{\lsub{P}{#1}_{#2}}
\newcommand{\bmat}[2]{{\mat{#1}_{#2}}}

% Vector spaces
\newcommand{\nomials}[1]{P_{#1}\par{\reals}}
\newcommand{\mats}[2]{\mathbb{M}_{#1,#2}\par{\reals}}

% Inner products
\newcommand{\iprod}[2]{\left< #1,#2 \right>}

% Common variables
\newcommand{\B}{\mathcal{B}}
\newcommand{\C}{\mathcal{C}}
\newcommand{\V}{\mathbb{V}}
\newcommand{\W}{\mathbb{W}}
\newcommand{\e}{\vec{e}}
\newcommand{\u}{\vec{u}}
\newcommand{\v}{\vec{v}}
\newcommand{\w}{\vec{w}}
\newcommand{\x}{\vec{x}}
\newcommand{\y}{\vec{y}}
\newcommand{\z}{\vec{z}}
\newcommand{\zero}{\vec{0}}


% CALCULUS
\newcommand{\ddx}[1]{\frac{d}{dx}\par{#1}}
\newcommand{\prm}{^\prime}
\newcommand{\pprm}{^{\prime\prime}}


% QUESTION-SPECIFIC
$$
