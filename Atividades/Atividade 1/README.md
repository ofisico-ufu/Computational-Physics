Esta atividade explorou a \textbf{implementação do algoritmo de gradiente descendente} para encontrar mínimos de funções, um método fundamental em otimização e aprendizado de máquina.

\subsection*{Exercício 1}
Implementação básica para a função quadrática $U(x) = x^2 - 1$, com análise da influência da \textbf{taxa de aprendizado ($\alpha$)} e \textbf{tolerância ($\epsilon$)} na convergência, incluindo visualização da trajetória da "partícula".

\subsection*{Exercício 2}
Aplicação do gradiente descendente à função $U(x) = x^2(x-1)(x+1)$, que possui múltiplos mínimos. Investigação da \textbf{sensibilidade da taxa de aprendizado} na convergência para diferentes mínimos.

\subsection*{Exercício 3}
Variação do Exercício 2 com a função $U(x) = x^2(x-1)(x+1) + x/4$, observando como a alteração na topografia da função afeta a convergência e a importância da escolha de $\alpha$.

\subsection*{Exercício 4}
Extensão do algoritmo para uma função bidimensional $U(x,y) = \sin(x)\cos(y) + 2(xy)^2/1000$. A visualização dos resultados incluiu \textbf{mapas de contorno} para a trajetória da partícula e gráficos da \textbf{evolução do valor da função ($U(x_n, y_n)$)} ao longo das iterações (epochs).