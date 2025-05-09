






```latex
\documentclass[border=10pt]{standalone} % <--- Border added here
\usepackage{tikz}
\usetikzlibrary{positioning, shapes.geometric, arrows.meta}

\begin{document}

\begin{tikzpicture}[
  node distance=1.2cm and 2cm,
  every node/.style={align=center, font=\small, draw, thick}
]

% Nodes
\node[shape=ellipse] (start) {Affective Modulation \\ (pre-agentive)};
\node[shape=ellipse, below=of start] (drift) {Semantic Drift \\ (in $\mathcal{F}$)};
\node[shape=rectangle, below=of drift] (bias) {Bias via Priors \\ $\pi_i$};

% Arrows
\draw[->, thick] (start) -- (drift);
\draw[->, thick] (drift) -- (bias);

\end{tikzpicture}

\end{document}
```



```latex
\documentclass[border=0pt]{standalone}
\usepackage{tikz}
\usetikzlibrary{positioning, shapes.geometric, arrows.meta}

\begin{document}

\begin{tikzpicture}[x=1cm, y=1cm]
  % Set explicit canvas size
  \useasboundingbox (0,0) rectangle (12,8); % 12cm wide, 8cm tall

  % Nodes
  \node[shape=ellipse, draw, align=center, font=\small] (start) at (6,7) {Affective Modulation \\ (pre-agentive)};
  \node[shape=ellipse, draw, align=center, font=\small] (drift) at (6,5.5) {Semantic Drift \\ (in $\mathcal{F}$)};
  \node[shape=rectangle, draw, align=center, font=\small] (bias) at (6,4) {Bias via Priors \\ $\pi_i$};

  % Arrows (using anchors!)
  \draw[->, thick] (start.south) -- (drift.north);
  \draw[->, thick] (drift.south) -- (bias.north);

\end{tikzpicture}

\end{document}
```
``