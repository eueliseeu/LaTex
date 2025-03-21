# Guia Profissional de LaTeX

Este documento apresenta uma visão geral dos principais comandos e estruturas utilizados em documentos LaTeX, com foco em boas práticas e referências úteis para aprofundamento.

---

## 1. Estrutura do Documento

A estrutura básica de um documento em LaTeX envolve:

- **`\documentclass{...}`**  
  Define o tipo de documento. Exemplos comuns incluem `article`, `report` e `book`.

- **`\usepackage{...}`**  
  Permite a inclusão de pacotes para funcionalidades extras. Alguns pacotes úteis são:  
  - `graphicx`: Inserção e manipulação de imagens.  
  - `amsmath`: Recursos avançados para escrita de fórmulas matemáticas.  
  - `hyperref`: Criação de links e referências clicáveis.

[Mais informações](https://www.overleaf.com/learn)

---

## 2. Cabeçalho e Informações do Documento

Defina as informações essenciais do seu documento:

- **`\title{...}`**  
  Define o título do documento.

- **`\author{...}`**  
  Indica o autor ou os autores.

- **`\date{...}`**  
  Especifica a data. Para utilizar a data atual, use `\date{\today}`.

- **`\maketitle`**  
  Insere o título, autor e data conforme definidos.

[Mais informações](https://www.overleaf.com/learn)

---

## 3. Organização do Documento

Organize o conteúdo em seções e subseções para melhorar a legibilidade:

- **`\section{...}`**  
  Cria uma seção principal.

- **`\subsection{...}`**  
  Cria uma subseção.

- **`\subsubsection{...}`**  
  Cria uma subsubseção.

- **`\paragraph{...}`**  
  Inicia um parágrafo com título.

- **`\tableofcontents`**  
  Gera automaticamente um índice com base nas seções.

[Mais informações](https://www.overleaf.com/learn)

---

## 4. Formatação de Texto

Utilize os comandos abaixo para realçar partes do texto:

- **`\textbf{...}`**: Texto em **negrito**.  
- **`\textit{...}`**: Texto em *itálico*.  
- **`\underline{...}`**: Texto sublinhado.  
- **`\emph{...}`**: Dá ênfase ao texto (geralmente em itálico).  
- **`\texttt{...}`**: Apresenta texto com formatação monoespaçada (ideal para códigos).  
- **`\footnote{...}`**: Adiciona uma nota de rodapé.

[Mais informações](https://www.overleaf.com/learn)

---

## 5. Trabalhando com Tabelas

Crie e formate tabelas com os seguintes ambientes e comandos:

- **`\begin{table}...\end{table}`**: Ambiente para tabelas.  
- **`\begin{tabular}{...}...\end{tabular}`**: Define uma tabela com colunas.  
  - `c`: Centralizado.  
  - `l`: Alinhado à esquerda.  
  - `r`: Alinhado à direita.  
  - `|`: Adiciona bordas verticais entre colunas.  
  - **`\hline`**: Insere uma linha horizontal.

[Mais informações](https://www.overleaf.com/learn)

---

## 6. Inserindo Figuras

Adicione imagens e figuras ao documento utilizando:

- **`\begin{figure}...\end{figure}`**: Ambiente para inserir figuras.  
- **`\includegraphics[...]{...}`**: Insere a imagem desejada.  
  - *Exemplo:* `[width=...]` define a largura da imagem.  
- **`\caption{...}`**: Adiciona uma legenda à figura.  
- **`\label{...}`**: Permite a criação de referências cruzadas.

[Mais informações](https://www.overleaf.com/learn)

---

## 7. Matemática no LaTeX

Para inserir fórmulas matemáticas, utilize os seguintes comandos:

- **Modo em Linha:**  
  Envolva a fórmula com `$ ... $`.

- **Modo de Exibição:**  
  Utilize `\[ ... \]` para fórmulas sem numeração ou  
  `\begin{equation}...\end{equation}` para fórmulas numeradas.

### Exemplos de símbolos matemáticos:
- Letras gregas: `\alpha`, `\beta`, `\gamma`.  
- Frações: `\frac{a}{b}`.  
- Somatório: `\sum`.  
- Integral: `\int`.

[Mais informações](https://www.overleaf.com/learn)

---

## 8. Listas

Crie listas de maneira organizada:

- **Listas com marcadores:**  
  ```latex
  \begin{itemize}
    \item Item 1
    \item Item 2
  \end{itemize}
  ```

- **Listas numeradas:**  
  ```latex
  \begin{enumerate}
    \item Primeiro item
    \item Segundo item
  \end{enumerate}
  ```

- **Listas descritivas:**  
  ```latex
  \begin{description}
    \item[Título] Descrição detalhada.
  \end{description}
  ```

[Mais informações](https://www.overleaf.com/learn)

---

## 9. Referências e Links

Gerencie referências e links dentro do documento:

- **`\label{...}`**  
  Define um rótulo para referências internas.

- **`\ref{...}`**  
  Faz referência a um rótulo previamente definido.

- **`\pageref{...}`**  
  Indica a página onde o rótulo se encontra.

- **`\url{...}`**  
  Insere um link clicável.

- **`\href{url}{texto}`**  
  Cria um link com texto personalizado (*requer o pacote `hyperref`*).

[Mais informações](https://www.overleaf.com/learn)

---

## 10. Gerenciamento de Páginas

Controlar a apresentação e numeração de páginas é fundamental:

- **`\footnote{...}`**  
  Adiciona notas de rodapé.

- **`\pagestyle{...}`**  
  Define o estilo dos cabeçalhos e rodapés (ex.: `plain`, `empty`, `headings`).

- **`\pagenumbering{...}`**  
  Altera o formato de numeração das páginas (ex.: `arabic`, `roman`).

[Mais informações](https://www.overleaf.com/learn)

---

## 11. Finalização do Documento

Finalize seu documento com o comando:

- **`\end{document}`**  
  Indica o fim do documento. Todo o conteúdo após esse comando será ignorado.

[Mais informações](https://www.overleaf.com/learn)
