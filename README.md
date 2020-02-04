# tex_exercise
This is a note to tex exercise.
%这是一个原始版本的tex模板

\documentclass[UTF8]{ctexart}
%这是导言区，可用来引入各种宏包

\usepackage{amsmath} % 这是用于数学公式编辑的宏包
\usepackage{fancyhdr} % 页眉页脚
\usepackage{lastpage} % 获得总页数
\usepackage{array} % 引入宏包，可对整列单元格进行修改
\usepackage{booktabs} % 三线表

\raggedright % 防止右边越界
% 首行缩进
\usepackage{indentfirst}
\setlength{\parindent}{2em} % 缩进两格

%插入图片的宏包
\usepackage{graphicx}
\graphicspath{{pic/}} % 在于.tex同级的目录下创建名为pic的文件夹

%%自定义页眉页脚
\pagestyle{fancy}
\lhead{\includegraphics[scale=0.1]{xiamen}}
%\chead{这是我的专用页眉}
\chead{\includegraphics[scale=0.1]{xiaoxun}}
%\rhead{\bfseries 右边页眉}
\rhead{\includegraphics[scale=0.1]{xueyuan}}
% \lfoot{页脚左边} \rfoot{右边页脚}
\cfoot{\thepage}

% 制作的封面
% 封面可放在导言区
\title{\textbf{\emph{这里是标题}}} %标题
\author{\underline{作者}} %作者
\date{\textit{\today}} %当前日期

% 接着是正文区

\begin{document}
	% 这是正文区，可用来编写文档
	
	\maketitle %此处生成封面
	% 可用(\newpage)生成新页
	
	% 这是摘要
	\begin{abstract} % 摘要
		这里是摘要
	\end{abstract}

	\tableofcontents % 生成目录
	
	\section{一}
		\subsection{第一节}
		\subsection{第二节}
	\section{二}
		\subsection{第一节}
		\subsection{第二节}
	\section{三}
		\subsection{第一节}
		\subsection{第二节}
	
	% 这是参考文献
	\begin{thebibliography}{99}
		
		% {article1、2、3}表示交叉引用命名
		
		\bibitem{article1}参考文献1: 参考文献1
		\bibitem{article2}参考文献2: 参考文献2
		\bibitem{article3}参考文献3: 参考文献3
	\end{thebibliography}
	
	
\end{document}
