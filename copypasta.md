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
\newcommand{\func}[2][]{\operatorname{ #2 }_{ #1 }\,}
\newcommand{\parfunc}[2][]{\operatorname{ #2 }_{ #1 }\par}

% Aligned ----------------------------------------------------------------------
\newcommand{\align}[1]{\begin{aligned} #1 \end{aligned}}

% Cases ------------------------------------------------------------------------
\newcommand{\cases}[1]{\begin{cases} #1 \end{cases}}
\newcommand{\if}[1]{\text{if \( #1 \)}}
\newcommand{\otherwise}{\text{otherwise}}
    \newcommand{\ow}{\otherwise}

% Slash Fraction ---------------------------------------------------------------
\newcommand{\flac}[2]{\left. #1 \middle/ #2 \right.}


% GENERAL UTILITIES ============================================================

% Left/Right aliases -----------------------------------------------------------
\newcommand{\tuple}{\pr}
\newcommand{\array}{\sq}
    \newcommand{\arr}{\sq}
\newcommand{\set}{\cb}
\newcommand{\abs}{\vv}
\newcommand{\size}{\vv}
\newcommand{\modulus}{\vv}
\newcommand{\norm}{\VV}
\newcommand{\length}{\VV}
\newcommand{\floor}{\fl}
\newcommand{\ceiling}{\cl}
    \newcommand{\ceil}{\cl}

% Miscellaneous ----------------------------------------------------------------
\newcommand{\defequals}{\mathrel{\mathop:}=}
    \newcommand{\defeq}{\defequals}
    \newcommand{\deq}{\defequals}
\newcommand{\pair}[2]{\tuple{ #1 , #2 }}
\newcommand{\range}[2]{{ #1 }\,{..}\,{ #2 }}
\newcommand{\index}[1]{\mathopen{} \sq{ #1 } \mathclose{}}
    \newcommand{\idx}{\index}
\newcommand{\divides}{\mid}


% COMPLEX NUMBERS ==============================================================

% Miscellaneous ----------------------------------------------------------------
\newcommand{\conjugate}[1]{\overline{#1}}
    \newcommand{\conj}{\conjugate}
\newcommand{\Realpart}[1][]{\parfunc[#1]{Re}}
    \newcommand{\Re}{\Realpart}
\newcommand{\Imaginarypart}[1][]{\parfunc[#1]{Im}}
    \newcommand{\Im}{\Imaginarypart}


% FLOATING POINT ===============================================================

% Miscellaneous ----------------------------------------------------------------
\newcommand{\float}{{fl}\par}
    % \newcommand{\fl}{\float} name conflict with floor
\newcommand{\repeat}[1]{\overline{ #1 }}
    \newcommand{\rep}{\repeat}
\newcommand{\machineepsilon}{\epsilon_{\mathit{mach}}}
    \newcommand{\emach}{\machineepsilon}

% Operators --------------------------------------------------------------------
\newcommand{\fplus}{\oplus}
    \newcommand{\fadd}{\fplus}
\newcommand{\fminus}{\ominus}
    \newcommand{\fsub}{\fminus}
\newcommand{\ftimes}{\otimes}
    \newcommand{\fmul}{\ftimes}
\newcommand{\fdivide}{\oslash}
    \newcommand{\fdiv}{\fdivide}


% SETS =========================================================================

% Set building notation --------------------------------------------------------
\newcommand{\where}{\ \middle|\ }

% Common sets ------------------------------------------------------------------
\newcommand{\Naturals}{\mathbb{N}}
    \newcommand{\Nats}{\Naturals}
    \newcommand{\N}{\Naturals}
\newcommand{\Integers}{\mathbb{Z}}
    \newcommand{\Ints}{\Integers}
    \newcommand{\Z}{\Integers}
\newcommand{\Reals}{\mathbb{R}}
    \newcommand{\R}{\Reals}
\newcommand{\Complex}{\mathbb{C}}
    \newcommand{\C}{\Complex}
\newcommand{\Polynomials}[2]{P_{ #1 }\par{ #2 }}
    \newcommand{\Nomials}{\Polynomials}
\newcommand{\Matrices}[3]{M_{ #1 , #2 }\par{ #3 }}
    \newcommand{\Mats}{\Matrices}

% Intervals --------------------------------------------------------------------
\newcommand{\cc}[2]{\left[ #1 , #2 \right]} % Closed-Closed
\newcommand{\co}[2]{\left[ #1 , #2 \right)} % Closed-Open
\newcommand{\oc}[2]{\left( #1 , #2 \right]} % Open-Closed
\newcommand{\oo}[2]{\left( #1 , #2 \right)} % Open-Open

% Set operations ---------------------------------------------------------------
\newcommand{\union}{\cup}
\newcommand{\Union}{\bigcup}
\newcommand{\intersect}{\cap}
\newcommand{\Intersect}{\bigcap}
\newcommand{\directsum}{\oplus}
    \newcommand{\dsum}{\directsum}


% LINEAR ALGEBRA ===============================================================

% Bases ------------------------------------------------------------------------
\newcommand{\Span}[1][]{\func[#1]{Span}}
\newcommand{\rank}[1][]{\parfunc[#1]{rank}}
\newcommand{\dim}[1][]{\parfunc[#1]{dim}}

% Matrices ---------------------------------------------------------------------
\newcommand{\matrix}[1]{{\begin{bmatrix} #1 \end{bmatrix}}}
    \newcommand{\mat}{\matrix}
\newcommand{\vector}{\matrix}
    \newcommand{\vect}{\vector}
\newcommand{\diagonal}[1][]{\parfunc[#1]{diag}}
    \newcommand{\diag}{\diagonal}
\newcommand{\trace}[1][]{\parfunc[#1]{tr}}
    \newcommand{\tr}{\trace}
\newcommand{\inverse}[1]{#1^{-1}}
    \newcommand{\inv}{\inverse}
\newcommand{\transpose}[1]{#1^{T}}
    \newcommand{\trans}{\transpose}
\newcommand{\conjtrans}[1]{#1^{*}}
	\newcommand{\conjt}{\conjtrans}
	\newcommand{\ctrans}{\conjtrans}
	\newcommand{\ct}{\conjtrans}

% Matrix subspaces -------------------------------------------------------------
\newcommand{\Columnspace}[1][]{\parfunc[#1]{Col}}
    \newcommand{\Colspace}{\Columnspace}
    \newcommand{\Col}{\Columnspace}
\newcommand{\Rowspace}[1][]{\parfunc[#1]{Row}}
    \newcommand{\Row}{\Rowspace}
\newcommand{\Nullspace}[1][]{\parfunc[#1]{Null}}
    \newcommand{\Null}{\Nullspace}
\newcommand{\LNullspace}[2][]{\Nullspace[#1]{\trans{ #2 }}}
    \newcommand{\LNull}{\LNullspace}

% Linear mappings --------------------------------------------------------------
\newcommand{\Range}[1][]{\parfunc[#1]{Range}}
\newcommand{\Kernel}[1][]{\parfunc[#1]{Ker}}
    \newcommand{\Ker}{\Kernel}
\newcommand{\nullity}[1][]{\parfunc[#1]{nullity}}

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
\newcommand{\projection}[1]{\parfunc[#1]{proj}}
    \newcommand{\proj}{\projection}
\newcommand{\perpendicular}[1]{\parfunc[#1]{perp}}
    \newcommand{\perp}{\perpendicular}
\newcommand{\orthogonalcomplement}[1]{{ #1 }^{\bot}}
    \newcommand{\orthocomplement}{\orthogonalcomplement}
    \newcommand{\orthocomp}{\orthogonalcomplement}
    \newcommand{\ocomp}{\orthogonalcomplement}

% Common linear algebra variables ----------------------------------------------
\newcommand{\B}{\mathcal{B}}
\newcommand{\U}{\mathbb{U}}
\newcommand{\V}{\mathbb{V}}
\newcommand{\W}{\mathbb{W}}
\newcommand{\a}{\vec{a}}
\newcommand{\b}{\vec{b}}
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
\newcommand{\dd}[3][]{\frac{d^{#1} {#2}}{d {#3}^{#1}}}
\newcommand{\pdd}[3][]{\frac{\delta^{#1} {#2}}{\delta {#3}^{#1}}}
\newcommand{\prm}{^\prime}
\newcommand{\pprm}{^{\prime\prime}}

% Logarithms
\newcommand{\lnp}{\ln\par}
\newcommand{\logp}[1][]{\log_{#1}\par}

% Trigonometry
\newcommand{\cosp}[1][]{\cos^{#1}\par}
\newcommand{\sinp}[1][]{\sin^{#1}\par}
\newcommand{\tanp}[1][]{\tan^{#1}\par}
\newcommand{\secp}[1][]{\sec^{#1}\par}
\newcommand{\cscp}[1][]{\csc^{#1}\par}
\newcommand{\cotp}[1][]{\cot^{#1}\par}


% GRAPHS =======================================================================

% Notation
\newcommand{\edge}{\pair}
\newcommand{\graph}{\pair}

% Vertices
\newcommand{\degree}[1][]{\parfunc[#1]{deg}}
    \newcommand{\deg}{\degree}
\newcommand{\indegree}[1][]{\parfunc[#1]{indegree}}
    \newcommand{\indeg}{\indegree}
    \newcommand{\ideg}{\indegree}
\newcommand{\outdegree}[1][]{\parfunc[#1]{outdegree}}
    \newcommand{\outdeg}{\outdegree}
    \newcommand{\odeg}{\outdegree}

% Trees
\newcommand{\BFS}[1][]{\parfunc[#1]{BFS}}
\newcommand{\DFS}[1][]{\parfunc[#1]{DFS}}
\newcommand{\level}[1][]{\parfunc[#1]{level}}
\newcommand{\parent}[1][]{\parfunc[#1]{parent}}

% Weighted Graphs
\newcommand{\weight}{w\par}

% Paths
\newcommand{\distance}[2]{d\par{ #1 , #2 }}
	\newcommand{\dist}{\distance}


% ALGORITHMS ===================================================================

% Big O Notation
\newcommand{\Oh}{O\par}
\newcommand{\oh}{o\par}
\newcommand{\Om}{\Omega\par}
\newcommand{\om}{\omega\par}
\newcommand{\Th}{\Theta\par}

% Decision Problems
\newcommand{\YES}{\text{YES}}
\newcommand{\NO}{\text{NO}}

% Complexity Classes
\newcommand{\reducesto}[1][]{\leq_{#1}}
\newcommand{\P}{\text{P}}
\newcommand{\NP}{\text{NP}}
\newcommand{\complete}[1]{\text{\(#1\)-complete}}
\newcommand{\SAT}[1]{\text{\(#1\)-SAT}}
\newcommand{\HamPath}{\text{Ham-Path}}

% Numerical Methods
\newcommand{\LTE}{{LTE}}


% LOGIC ========================================================================

% Values
\newcommand{\true}{\text{true}}
\newcommand{\True}{\text{True}}
\newcommand{\TRUE}{\text{TRUE}}
\newcommand{\false}{\text{false}}
\newcommand{\False}{\text{False}}
\newcommand{\FALSE}{\text{FALSE}}

% Operators
\newcommand{\AND}{\and}
\newcommand{\OR}{\or}
\newcommand{\NOT}{\neg}
$$
