\documentclass[]{resume-openfont}

\pagestyle{fancy}
\resetHeaderAndFooter

%--------------------------------------------------------------
% Convenience command - make it easy to fill template

% Create job position command. Parameters: company, position, location, when
\newcommand{\resumeHeading}[4]{\runsubsection{\uppercase{#1}}\descript{ | #2}\hfill\location{#3 | #4}\fakeNewLine}

% Create education heading. Parameters: Name, degree, location, when
\newcommand{\educationHeading}[4]{\runsubsection{#1}\hspace*{\fill}  \location{#3 | #4}\\
\descript{#2}\fakeNewLine}

% Create project heading. Parameters: Name, link, Tech stack
\newcommand{\projectHeading}[3]{\Project{#1}{#2} % Link is #2
\descript{#3}\\} % Tech stack is #3

\newcommand{\projectHeadingWithDate}[4]{\Project{#1}{#2} % Link is #2
\descript{#3 | #4}\\} % Tech stack is #3, Date is #4

% Parameters: courses
\newcommand{\courseWork}[1]{\textbf{Coursework:} #1}

\newcommand{\Cgpa}[1]{\textbf{Cgpa:} #1}
 
%--------------------------------------------------------------
\begin{document}

%--------------------------------------------------------------
%       Profile
%--------------------------------------------------------------
\newcommand{\yourName}{Chirag Singh} % First Last
% How you want it to show up on the resume
% \newcommand{\yourWebsite}{yourwebsite.com}
% vs how you want it to show up. If it's the same you can just replace "\yourWebsiteLink" with "yourWebsite"
\newcommand{\yourEmail}{chiragdhouni20@gmail.com} % someEmail@edu.com
\newcommand{\yourPhone}{+91 8826882876} % 1-234-567-890
\newcommand{\githubUserName}{chirag405} % myGithubName
\newcommand{\linkedInUserName}{chirag404} % linkedInUsername

% An alternate profile section 
% \alignProfileTable
% \begin{tabular*}{\textwidth}{l@{\extracolsep{\fill}}r}
%      \ralewayBold{\href{\yourWebsiteLink}{\Large \yourName}} & 
%      Email : \href{mailto:\yourEmail}{\yourEmail}
%      \\
%      \href{https://github.com/\githubUserName}{GitHub://\githubUserName} & 
%      Mobile : \yourPhone
%      \\
%      \href{https://www.linkedin.com/in/\linkedInUserName}{LinkedIn://\linkedInUserName} & Website : \href{\yourWebsiteLink}{\yourWebsite}
%      \\
% \end{tabular*}

\begin{center}
    \Huge \scshape \latoRegular{\yourName} \\ \vspace{1pt}
    \small \href{mailto:\yourEmail}{\underline{\yourEmail}}  $|$  \yourPhone $|$ 
    \href{https://www.linkedin.com/in/\linkedInUserName}{\underline{linkedin/\linkedInUserName}} $|$
    \href{https://github.com/\githubUserName}{\underline{github/\githubUserName}} 
    % $|$ \href{\yourWebsiteLink}{\underline{\yourWebsite}} % Uncomment if you have a personal website
\end{center}

%--------------------------------------------------------------
%       Education
%--------------------------------------------------------------
\section{Education}
% Put school first and degree second if your school is reputable
\educationHeading{Raj Kumar Goel Institute Of Technology}{B.Tech  Computer Science}{Ghaziabad, India}{2021-2025}

\Cgpa{7.7/10}
% \courseWork{Data Structures and Algorithms; Operating Systems;  Computer Security; Software Testing; Advanced Networking; Big Data Analytics} % Example coursework
\sectionsep

%--------------------------------------------------------------
%       Experience
%--------------------------------------------------------------
\section{Work Experience}
\resumeHeading{Higroove Systems}{Flutter Developer Intern}{New Delhi, India}{June 2025 – Sept 2025}
\begin{bullets}
    \item Reduced API response calls and response time by 40% using
Hive local database for efficient storage and retrieval

    \item Optimized background processes and battery usage with BloC

    \item Developed 5 fully functional Flutter apps.
    \item Collaborated with Android team to build native features using Kotlin
\end{bullets}
\sectionsep

%--------------------------------------------------------------
%       Projects
%--------------------------------------------------------------
\section{Projects}

\projectHeading{SayWhat}{https://github.com/yourGithub/project1}{Tech Stack: Python, Flask, React, Docker}
\begin{bullets}
    \item Developed a key feature that improved user engagement by X%.
    \item Implemented a scalable backend API using Flask and deployed it with Docker.
    \item Designed and built a responsive user interface with React and Material UI.
\end{bullets}
\sectionsep
  
\projectHeading{Tool X}{https://github.com/yourGithub/project2}{Tech Stack: Java, Spring Boot, PostgreSQL, AWS}
\begin{bullets}
    \item Engineered a microservice architecture for enhanced modularity and fault tolerance.
    \item Utilized PostgreSQL for data persistence and optimized complex queries.
    \item Deployed the application on AWS EC2 with S3 for static storage.
\end{bullets}
\sectionsep

\projectHeading{UpCraft}{https://github.com/yourGithub/project3}{Tech Stack: C++, Unreal Engine, AI}
\begin{bullets}
    \item Created an AI system for non-player characters (NPCs) using behavior trees in Unreal Engine.
    \item Implemented advanced pathfinding algorithms for realistic agent movement.
    \item Optimized game performance for smoother gameplay on target hardware.
\end{bullets}
\sectionsep

%--------------------------------------------------------------
%       Publications
%--------------------------------------------------------------
\section{Publications}
\runsubsection{\href{https://doi.org/your_doi_link_here}{Title of Your Groundbreaking Research Paper}}
\descript{Authors: [Your Name], Co-author One, Co-author Two (Month Year). *Journal of Fictional Computer Science / Proceedings of Esteemed Conference*, Vol. X, No. Y, pp. 123-456. Presented at An Important Conference (if applicable).}
\fakeNewLine
\sectionsep

%--------------------------------------------------------------
%       Achievements
%--------------------------------------------------------------
\section{Achievements}
\begin{bullets}
    \item Finalist – Uyir Road Safety
Hackathon 2025 ( top 10
among 3000 teams)
    \item 1st Prize – College Coding
Championship 2022
    \item LeetCode 700+
    
\end{bullets}
\sectionsep

%--------------------------------------------------------------
%       Skills
%--------------------------------------------------------------
\section{Skills}
\begin{skillList}
    \singleItem{Languages:}{ Python, C++, JavaScript, TypeScript, SQL, Dart, Nodejs} % Add your languages
    \\
    \singleItem{CS Fundamentals:}{Operating Systems, Computer Networks, DBMS, OOP, DSA} % Add your web dev skills
    \\
    \singleItem{Technologies/Frameworks:}{React, Flutter,Git, Nextjs, React Native, LangChain, CrewAi, Docker, GCP,  TensorFlow} % Add relevant technologies
    \\
    \singleItem{Databases:}{MySQL, PostgreSQL, MongoDB, Supabase, AppWrite, convex, Firebase} % Add your database skills
\end{skillList}

% A more concise alternate 
% \begin{skillList}
%      \doubleItem{Languages:}{Java, C++, Python, C\#, PHP, Prolog, Bash, C, Racket}%
%      {Databases:}{SQL, MongoDB, Neo4j, DynamoDB}
%      \\
%      \doubleItem{Web Development:}{JavaScript, TypeScript, React, HTML/CSS}
%      {Technology:}{Git, AWS, GCP, Azure, Docker, \LaTeX}%
% \end{skillList}
\end{document}
