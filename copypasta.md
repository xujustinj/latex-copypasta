$$
% LaTeX UTILITIES ==============================================================

% Left/Right -------------------------------------------------------------------
% These two-letter command names mostly come from old personal conventions.
\newcommand{\pr}[1]{\left( #1 \right)} % PaRentheses
\newcommand{\sq}[1]{\left[ #1 \right]} % SQuare brackets
\newcommand{\cb}[1]{\left\lbrace #1 \right\rbrace} % Curly Braces
\newcommand{\vv}[1]{\left\lvert #1 \right\rvert} % single pipes (vert vert)
\newcommand{\VV}[1]{\left\lVert #1 \right\rVert} % double pipes (Vert Vert)
\newcommand{\ag}[1]{\left\langle #1 \right\rangle} % AnGle brackets
\newcommand{\fl}[1]{\left\lfloor #1 \right\rfloor} % FLoor
\newcommand{\cl}[1]{\left\lceil #1 \right\rceil} % CeiLing

% Left scripts -----------------------------------------------------------------
\newcommand{\lsub}[2]{{\vphantom{ #1 }}_{ #2 } #1}
\newcommand{\lsup}[2]{{\vphantom{ #1 }}^{ #2 } #1}
\newcommand{\lsubp}[2]{{\vphantom{ #1 }}_{ #2 }^{ #3 } #1}

% Functions --------------------------------------------------------------------
\newcommand{\par}[1]{\mathopen{} \pr{ #1 } \mathclose{}} % PARameter
\newcommand{\func}[1]{\operatorname{ #1 }\,}
\newcommand{\funcsub}[2]{\operatorname{ #1 }_{ #2 }\,}
\newcommand{\parfunc}[1]{\operatorname{ #1 }\par}
\newcommand{\parfuncsub}[2]{\operatorname{ #1 }_{ #2 }\par}

% Cases ------------------------------------------------------------------------
\newcommand{\if}[1]{\text{if \( #1 \)}}
\newcommand{\otherwise}{\text{otherwise}}
    \newcommand{\ow}{\otherwise}


% GENERAL UTILITIES ============================================================

% Left/Right aliases -----------------------------------------------------------
\newcommand{\array}{\sq}
    \newcommand{\arr}{\sq}
\newcommand{\index}[1]{\mathopen{} \sq{ #1 } \mathclose{}}
    \newcommand{\idx}{\index}
\newcommand{\set}{\cb}
\newcommand{\abs}{\vv}
\newcommand{\size}{\vv}
\newcommand{\norm}{\VV}
\newcommand{\length}{\VV}
\newcommand{\floor}{\fl}
\newcommand{\ceiling}{\cl}
    \newcommand{\ceil}{\cl}

% Miscellaneous-----------------------------------------------------------------
\newcommand{\defequals}{\mathrel{\mathop:}=}
    \newcommand{\defeq}{\defequals}
    \newcommand{\deq}{\defequals}
\newcommand{\range}[2]{{ #1 }\,{..}\,{ #2 }}


% SETS =========================================================================

% Set building notation --------------------------------------------------------
\newcommand{\where}{\ \middle|\ }

% Common sets ------------------------------------------------------------------
\newcommand{\Naturals}{\mathbb{N}}
\newcommand{\Nats}{\Naturals}
\newcommand{\N}{\Naturals}
\newcommand{\Reals}{\mathbb{R}}
\newcommand{\R}{\Reals}
\newcommand{\Polynomials}[2]{P_{ #1 }\par{ #2 }}
\newcommand{\Nomials}{\Polynomials}
\newcommand{\Matrices}[3]{\mathbb{M}_{ #1 , #2 }\par{ #3 }}
\newcommand{\Mats}{\Matrices}

% Intervals --------------------------------------------------------------------
\newcommand{\cc}[2]{\left[ #1 , #2 \right]} % Closed-Closed
\newcommand{\co}[2]{\left[ #1 , #2 \right)} % Closed-Open
\newcommand{\oc}[2]{\left( #1 , #2 \right]} % Open-Closed
\newcommand{\oo}[2]{\left( #1 , #2 \right)} % Open-Open

% Set operations ---------------------------------------------------------------
\newcommand{\union}{\cup}
\newcommand{\intersect}{\cap}


% LINEAR ALGEBRA ===============================================================

% Bases ------------------------------------------------------------------------
\newcommand{\Span}{\func{Span}}
\newcommand{\rank}{\parfunc{rank}}
\newcommand{\dim}{\parfunc{dim}}

% Matrices ---------------------------------------------------------------------
\newcommand{\matrix}[1]{{\begin{bmatrix} #1 \end{bmatrix}}}
    \newcommand{\mat}{\matrix}
\newcommand{\vector}{\matrix}
	\newcommand{\vect}{\vector}
\newcommand{\diagonal}{\parfunc{diag}}
    \newcommand{\diag}{\diagonal}
\newcommand{\trace}{\parfunc{tr}}
    \newcommand{\tr}{\trace}
\newcommand{\inverse}[1]{{ #1 }^{-1}}
    \newcommand{\inv}{\inverse}
\newcommand{\transpose}[1]{{ #1 }^{T}}
    \newcommand{\trans}{\transpose}

% Matrix subspaces -------------------------------------------------------------
\newcommand{\Columnspace}{\parfunc{Col}}
    \newcommand{\Colspace}{\Columnspace}
    \newcommand{\Col}{\Columnspace}
\newcommand{\Rowspace}{\parfunc{Row}}
    \newcommand{\Row}{\Rowspace}
\newcommand{\Nullspace}{\parfunc{Null}}
    \newcommand{\Null}{\Nullspace}
\newcommand{\LNullspace}[1]{\Nullspace{\trans{ #1 }}}
    \newcommand{\LNull}{\Lnullspace}

% Linear mappings --------------------------------------------------------------
\newcommand{\Range}{\parfunc{Range}}
\newcommand{\Kernel}{\parfunc{Ker}}
    \newcommand{\Ker}{\Kernel}
\newcommand{\nullity}{\parfunc{nullity}}

% Coordinates ------------------------------------------------------------------
\newcommand{\coordinates}[2]{\matrix{ #1 }_{ #2 }}
    \newcommand{\coords}{\coordinates}
\newcommand{\changecoordinates}[2]{\lsub{P}{ #1 }_{ #2 }}
    \newcommand{\coc}{\changecoordinates}
% matrix of #2 w.r.t. bases #3 and #1
\newcommand{\mapmatrix}[3]{\lsub{\matrix{ #2 }}{ #1 }_{ #3 }}
    \newcommand{\mapmat}{\mapmatrix}
\newcommand{\bmatrix}[2]{{\mat{ #1 }_{ #2 }}}
    \newcommand{\bmat}{\bmatrix}

% Inner products ---------------------------------------------------------------
\newcommand{\innerproduct}[2]{\ag{ #1 , #2 }}
    \newcommand{\innerprod}{\innerproduct}
    \newcommand{\iprod}{\innerproduct}
\newcommand{\projection}{\parfuncsub{proj}}
    \newcommand{\proj}{\projection}
\newcommand{\perpendicular}{\parfuncsub{perp}}
    \newcommand{\perp}{\perpendicular}
\newcommand{\orthogonalcomplement}[1]{{ #1 }^{\bot}}
    \newcommand{\orthocomplement}{\orthogonalcomplement}
    \newcommand{\orthocomp}{\orthogonalcomplement}
    \newcommand{\ocomp}{\orthogonalcomplement}

% Common linear algebra variables ----------------------------------------------
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


% CALCULUS =====================================================================

% Derivative notations
\newcommand{\ddx}[1]{\frac{d}{dx}\par{ #1 }}
\newcommand{\prm}{^\prime}
\newcommand{\pprm}{^{\prime\prime}}
$$
