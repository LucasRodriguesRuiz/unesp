# 🧮 Introdução às Matrizes

---

## 📖 Definição e Notação

**Definição:** Uma matriz é uma tabela de números reais de ordem (tamanho) $m \times n$, sendo $m$ o número de **linhas** e $n$ o número de **colunas**. 
> **Nota:** Quando $m = n$ (o número de linhas é igual ao de colunas), a matriz é chamada de matriz quadrada e, geralmente, seu tamanho é representado por um único número (ex: matriz de ordem $n$).

- **Nomes de Matrizes:** São sempre dados por letras **maiúsculas** (ex: $A, B, M$).
- **Notação de Elementos:** Os elementos de uma matriz são representados por letras minúsculas seguidas de índices indicando sua posição: $a_{ij}$.
  - Onde $i$ representa a linha ($1 \leq i \leq m$).
  - Onde $j$ representa a coluna ($1 \leq j \leq n$).
**Notação Geral de uma Matriz:**
$$
A = \begin{bmatrix}
a_{11} & a_{12} & \dots & a_{1n} \\
a_{21} & a_{22} & \dots & a_{2n} \\
\vdots & \vdots & \ddots & \vdots \\
a_{m1} & a_{m2} & \dots & a_{mn}
\end{bmatrix}
$$

**Exemplo de uma Matriz Genérica $3 \times 3$:**
$$
\begin{bmatrix}
a_{11} & a_{12} & a_{13} \\
a_{21} & a_{22} & a_{23} \\
a_{31} & a_{32} & a_{33}
\end{bmatrix}
$$

---

## ⭐ Matrizes Especiais

### ➖ Matriz Linha
Possui apenas **uma** linha ($1 \times n$).
$$
L =
\begin{bmatrix}
3 & 7 & -4 & 0 & \frac{2}{5}
\end{bmatrix}_{1 \times 5}
$$

### ⏐ Matriz Coluna
Possui apenas **uma** coluna ($m \times 1$).
$$
P_{4 \times 1} =
\begin{bmatrix}
7 \\ 2 \\ 0.5 \\ -4
\end{bmatrix}
$$

### ∅ Matriz Nula
Todos os seus elementos são iguais a zero. Pode ser de qualquer ordem.
$$
M_{4 \times 3} =
\begin{bmatrix}
0 & 0  & 0 \\
0 & 0  & 0 \\
0 & 0  & 0 \\
0 & 0  & 0
\end{bmatrix}
$$

### ◻️ Matriz Quadrada
O número de linhas é exatamente igual ao de colunas ($m = n$).
$$
M_{3 \times 3} = M_3 =
\begin{bmatrix}
\log 3 & \sin \pi  & 0.5 \\
7 & \frac{3}{7}  & \cos \frac{3\pi}{2} \\
-2 & \frac{10}{3}  & -10
\end{bmatrix}
$$

### ↘️ Matriz Diagonal
É toda matriz quadrada em que os elementos que **não** pertencem à diagonal principal são iguais a zero.
$$
\begin{bmatrix}
2 & 0  & 0 \\
0 & 1  & 0 \\
0 & 0  & -3 
\end{bmatrix},
\quad
\begin{bmatrix}
3 & 0  \\
0 & -2  \\
\end{bmatrix},
\quad
\begin{bmatrix}
0 & 0  & 0 & 0\\
0 & 0  & 0 & 0\\
0 & 0  & 0 & 0\\
0 & 0  & 0 & 0
\end{bmatrix}
$$

### 🆔 Matriz Identidade (Unidade)
É toda matriz quadrada diagonal onde **todos** os elementos da diagonal principal são iguais a $1$. É comumente representada pela letra $I$.
$$
I_2=
\begin{bmatrix}
1 & 0  \\
0 & 1  \\
\end{bmatrix},
\quad
I_3=
\begin{bmatrix}
1 & 0  & 0 \\
0 & 1  & 0 \\
0 & 0  & 1
\end{bmatrix},
\quad
I_4=
\begin{bmatrix}
1 & 0  & 0 & 0\\
0 & 1  & 0 & 0\\
0 & 0  & 1 & 0\\
0 & 0  & 0 & 1
\end{bmatrix}
$$

### 📐 Matriz Triangular
Matrizes quadradas onde os elementos acima ou abaixo da diagonal principal são todos nulos.

**Triangular Inferior** (zeros acima da diagonal):
$$
A = \begin{bmatrix}
a_{11} & 0 & \dots & 0 \\
a_{21} & a_{22} & \dots & 0 \\
\vdots & \vdots & \ddots & \vdots \\
a_{n1} & a_{n2} & \dots & a_{nn}
\end{bmatrix}
$$

**Triangular Superior** (zeros abaixo da diagonal):
$$
A = \begin{bmatrix}
a_{11} & a_{12} & \dots & a_{1n} \\
0 & a_{22} & \dots & a_{2n} \\
\vdots & \vdots & \ddots & \vdots \\
0 & 0 & \dots & a_{nn}
\end{bmatrix}
$$

---

## ✖️ Diagonais de Matrizes Quadradas

Em matrizes quadradas (ordem $n$), podemos identificar duas diagonais importantes:

### 1️⃣ Diagonal Principal
É formada pelos elementos onde o índice da linha é igual ao índice da coluna ($i = j$).
> **Fórmula (Conjunto):**  
> $\{a_{ij} \mid i = j\} = \{a_{11}, a_{22}, a_{33}, a_{44}, \dots, a_{nn}\}$

### 2️⃣ Diagonal Secundária
É formada pelos elementos onde a soma dos índices da linha e da coluna é igual à ordem da matriz mais um ($i + j = n + 1$).
> **Fórmula (Conjunto):**  
> $\{a_{ij} \mid i + j = n + 1\} = \{a_{1n}, a_{2, n-1}, a_{3, n-2}, \dots, a_{n1}\}$

---

## 🟰 Igualdade de Matrizes

Sejam $A = (a_{ij})_{m \times n}$ e $B = (b_{ij})_{m \times n}$ duas matrizes da **mesma ordem**. Elas são iguais se, e somente se, todos os seus elementos correspondentes forem iguais:

$$
A = B \iff a_{ij} = b_{ij}, \quad \forall i, j
$$

### 📌 Exemplos de Igualdade

**1. Matrizes definidas iguais:**
Apesar de escritas de formas diferentes (usando frações e raízes), os resultados de cada posição são idênticos.
$$
\begin{bmatrix} 1 & 2 \\ 3 & 4 \end{bmatrix} = \begin{bmatrix} 1 & \frac{4}{2} \\ \sqrt{9} & 2^2 \end{bmatrix}
$$

**2. Matrizes definidas diferentes:**
Mesmo tendo vários números parecidos, basta que **um único** elemento correspondente seja diferente para que as matrizes não sejam iguais (neste caso, o elemento $a_{22}$).
$$
\begin{bmatrix} 1 & 0 \\ 0 & 1 \end{bmatrix} \neq \begin{bmatrix} 1 & 0 \\ 0 & -1 \end{bmatrix}
$$

**3. Matrizes com variáveis (Encontrando a solução):**
Dadas as matrizes $E$ e $F$, descubra os valores de $x$ e $y$ para que $E = F$.
$$
E = \begin{bmatrix} x & 5 \\ 4 & y+1 \end{bmatrix}, \quad F = \begin{bmatrix} 2 & 5 \\ 4 & 7 \end{bmatrix}
$$
> **Solução:**  
> Para serem iguais, os elementos nas mesmas posições devem ser idênticos.  
> $a_{11} = b_{11} \implies \mathbf{x = 2}$  
> $a_{22} = b_{22} \implies y + 1 = 7 \implies \mathbf{y = 6}$

---

## 📝 Exercícios Resolvidos

**1) Indique explicitamente os elementos da matriz $A = (a_{ij})_{3 \times 3} \rightarrow a_{ij} = i - j$**

$$
\begin{bmatrix}
a_{11} & a_{12}  & a_{13} \\
a_{21} & a_{22}  & a_{23} \\
a_{31} & a_{32}  & a_{33}
\end{bmatrix}
=
\begin{bmatrix}
1-1 & 1-2  & 1-3 \\
2-1 & 2-2  & 2-3 \\
3-1 & 3-2  & 3-3 
\end{bmatrix}
=
\begin{bmatrix}
0 & -1  & -2 \\
1 & 0  & -1 \\
2 & 1  & 0 
\end{bmatrix}
$$

**2) Escreva a matriz $A = (a_{ij})_{2 \times 3} \rightarrow a_{ij} = \begin{cases} i+2j, & \text{se } i > j \\ i^j, & \text{se } i = j \\ 2i-j, & \text{se } i < j \end{cases}$**

Calculando posição por posição com as regras dadas:
- $a_{11} (i=j): 1^1 = 1$
- $a_{12} (i<j): 2(1)-2 = 0$
- $a_{13} (i<j): 2(1)-3 = -1$
- $a_{21} (i>j): 2+2(1) = 4$
- $a_{22} (i=j): 2^2 = 4$
- $a_{23} (i<j): 2(2)-3 = 1$

$$
A =
\begin{bmatrix}
1 & 0 & -1 \\
4 & 4 & 1
\end{bmatrix}
$$

**3) Construa a matriz real quadrada A de ordem 3, definida por: $a_{ij} = \begin{cases} 2^{i+j}, & \text{se } i < j \\ i^2-j+1, & \text{se } i \ge j \end{cases}$**

Aplicando as regras para a matriz $3 \times 3$:
$$
A =
\begin{bmatrix}
1 & 8  & 16 \\
4 & 3  & 32 \\
9 & 8  & 7 \\
\end{bmatrix}
$$