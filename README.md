# texsimple
first try
#------------------------------------------------------------------------------------------------------------------------------------------------------
\documentclass[12pt]{report}
\usepackage[a4paper]{geometry}
\usepackage[myheadings]{fullpage}
\usepackage{fancyhdr}
\usepackage{lastpage}
\usepackage{graphicx, wrapfig, subcaption, setspace, booktabs}
\usepackage[T1]{fontenc}
\usepackage[font=small, labelfont=bf]{caption}
\usepackage{fourier}
\usepackage[protrusion=true, expansion=true]{microtype}
\usepackage[french]{babel}
\usepackage{sectsty}
\usepackage{url, lipsum}
\usepackage[T1]{fontenc}
\usepackage{fancybox}
\usepackage{graphicx}
\usepackage{floatflt}
\usepackage{float}
\usepackage{longtable}
\usepackage{supertabular}
\usepackage{fourier-orns}
\usepackage{array}
\usepackage{frcursive}
\usepackage{amsmath}
\usepackage{amsfonts}
\usepackage{multicol}
\usepackage{listings}
\usepackage{fancyhdr}
\usepackage{multirow}
\usepackage{color}
\usepackage{xcolor}
\usepackage{wrapfig}
\usepackage[nottoc, notlof, notlot]{tocbibind}
\usepackage{enumerate}
\usepackage{enumitem}
\usepackage{pslatex}
\usepackage[utf8x]{inputenc}
\usepackage[colorinlistoftodos]{todonotes}
\usepackage{pdfpages}
\usepackage{etex}
\usepackage{lscape}
\usepackage{hyperref}
%\usepackage[dvipsnames]{xcolor}

\hypersetup{                    % parametrage des hyperliens
    colorlinks=true,                % colorise les liens
    breaklinks=true,
                % permet les retours à la ligne pour les liens trop longs
    urlcolor= blue,                 % couleur des hyperliens
    linkcolor= black,                % couleur des liens internes aux documents (index, figures, tableaux, equations,...)
    citecolor= green                % couleur des liens vers les references bibliographiques
    }


\newcommand{\HRule}[1]{\rule{\linewidth}{#1}}
\renewcommand{\thesection}{\Roman{section}.}
\renewcommand{\thesubsection}{ \arabic{subsection})}


\onehalfspacing
\setcounter{tocdepth}{5}
\setcounter{secnumdepth}{5}

%-------------------------------------------------------------------------------
% HEADER & FOOTER
%-------------------------------------------------------------------------------
\pagestyle{fancy}
\fancyhf{}
\setlength\headheight{2pt}
\fancyhead[L]{\bsc{toto, toto, toot, toto, toto}}
\fancyhead[R]{\bsc{EISTI Pau}}
\fancyfoot[R]{\thepage\ / \pageref{LastPage}}
%-------------------------------------------------------------------------------
% TITLE PAGE
%-------------------------------------------------------------------------------

\begin{document}
\vspace{-12pt}
\begin{figure}
	 \begin{center}
		\includegraphics[scale=0.3]{Pictures/image}
	 \end{center}
\end{figure}

\title{  \textsc{Mini projet JEE}
		\HRule{0.5pt} \\
		\LARGE \textbf{\uppercase{Le Mauvais Coin}}
		\HRule{2pt} \\ [1.5cm]
%        \includegraphics[width=0.20\textwidth]{EISTI.jpg}~\\[0cm]
		\normalsize \vspace*{1\baselineskip}}
		
\date{18/11/2014}

 

\author{
		\bsc{toto} toto, \bsc{toto} toto, \bsc{toto} toto, \\
        \bsc{toto} -toto, \bsc{toto} toto \\   
        ecole }
                

\maketitle
\tableofcontents
\newpage

%-------------------------------------------------------------------------------
% Section title formatting
\sectionfont{\scshape}
%-------------------------------------------------------------------------------
\definecolor{mail}{rgb}{0,0,0.75} %Couleur des adresses mails
%-------------------------------------------------------------------------------
% BODY
%-------------------------------------------------------------------------------

\section{Introduction}
\vspace{1cm}

\newpage
\section{Rappel du sujet}

\subsection{Besoins}

\subsection{Contraintes}


\newpage
\section{Ressources}

\subsection*{Présentation de l'équipe}
	Notre équipe de travail est composée de cinq élèves ingénieurs (ING2) pour réaliser ce projet de la matière Java-EE. 
\\
\\
\noindent toto toto :
		\begin{itemize}
			\item Contact :\textcolor{mail}{toto@toto.eu}
			\\
		\end{itemize} 
	

\subsection*{Ressources matérielles}


\subsection*{Ressources financières}


\newpage
\section{Fonctionnalités}

\subsubsection*{Connexion}

\begin{center}
		\includegraphics[scale=0.5]{Pictures/accueil.png}
\end{center}

\begin{center}
		\includegraphics[scale=0.5]{Pictures/inscription.png}
\end{center}

\subsubsection*{Vente}
Un utilisateur connecté va pouvoir mettre en ligne des objets pour les vendre. Il lui suffit d'ajouter une annonce en renseignant les informations nécessaires comme un titre, une description et un prix s'il s'agit d'une vente (ou la description des objets contre lesquels il voudrait échanger le sien s'il s'agit d'un échange). Un objet est soit vendu, soit échangé, soit donné.\\

Une fois qu'un utilisateur a mis en ligne des objets, il peut consulter les annonces qu'il a passées. \\

Quant aux propositions que le vendeur reçoit, il pourra choisir d'accepter ou non celles-ci. Une fois une proposition acceptée, un déclencheur dans la base de données met à jour les propositions concernant cet objet en passant le statut de celle acceptée à "accepte" et celui des autres à "refuse". Les informations de l'objet se mettent également à jour puisqu'il passe à l'état de vendu.

\begin{center}
		\includegraphics[scale=0.5]{Pictures/vendeur.png}
\end{center}

\subsubsection*{Achat}  
.

\subsubsection*{Diagramme Use Case}
Pour schématiser les principales fonctionnalités de l'application, nous avons réalisé un diagramme de Use Case \hyperref[UseCase]{\underline{disponible ici}.}

\begin{figure}[htbp]
		\centering
			\includegraphics[scale=0.8]{Pictures/usecase.jpg}
			\caption{\label{UseCase}Diagramme Use Case}
			
	\end{figure}



%\newpage
%\hyperref[MCD]{\underline{Modèle Conceptuel de Données} \\

\begin{landscape}
	%Image centree
	%width=20cm, height=15cm
	\begin{figure}[htbp]
		\centering
			\includegraphics[scale=0.8]{Pictures/mcd1.PNG}
			\caption{\label{MCD}Modèle Conceptuel de Données}
			
	\end{figure}
\end{landscape}

\newpage
\subsection{\label{hibernate}Hibernate}


\begin{figure}[htbp]
		\centering
			\includegraphics[scale=1]{Pictures/mvc.PNG}
			\caption{\label{MVC}Pattern MVC}
			
	\end{figure}


\newpage
\section{Conclusion}
 l'annexe B: \hyperref[dev]{\underline{Manuel Développeur}} 

\newpage
\appendix
\chapter{Manuel utilisateur}

\section{Base de Données}

\newpage
\section{Application Java}


\newpage
\chapter{\label{dev}Manuel Développeur}

\subsection*{Fonctionnalités non gérées}


\subsection*{Améliorations disponibles rapidement}


\end{document}
#----------------------------------------------------------------------------------------------------------
