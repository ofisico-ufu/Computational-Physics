# Estrutura de Bandas em Cristais Unidimensionais

Nesta atividade, exploramos a estrutura de bandas de um cristal unidimensional resolvendo a equação de Schrödinger independente do tempo, utilizando uma expansão da função de Bloch no espaço-$k$. O objetivo foi construir e diagonalizar a Hamiltoniana para diferentes valores de $k$ dentro da 1ª zona de Brillouin, analisando como os parâmetros de acoplamento e potencial influenciam a forma e os gaps das bandas de energia.

Foi implementado um código em Python para montar a matriz de Hamiltoniana em uma base de ondas planas ($e^{iGx}$), variando o número de vetores-$G$ e o parâmetro de acoplamento $\alpha$. Os autovalores obtidos da diagonalização fornecem as energias permitidas (bandas) para cada valor de $k$.

---

## Exercício 6.1

Construímos uma matriz Hamiltoniana $5 \times 5$ com:

- Diagonal principal: $H_{ii} = (k - 2\pi n_i)^2$
- Termos de acoplamento: $H_{0,4} = H_{4,0} = 2.0$ (entre $n = \pm2$) e $H_{1,3} = H_{3,1} = 2.0$ (entre $n = \pm1$)
- Os demais termos definidos como zero.

A diagonalização dessa matriz para valores de $k \in [-\pi, \pi]$ forneceu o diagrama de bandas com gaps definidos pelos acoplamentos $\alpha$.

---

## Exercício 6.2

Calculamos os elementos de uma nova matriz potencial $V_{5 \times 5}$ com amplitude $A = 3$ e frequência $q = 0{,}5$, segundo:

$$
V_{m,n} = \int_0^1 A \cos(2\pi q x) \cdot e^{i 2\pi (m-n)x} \, dx
$$

Essa matriz contém acoplamentos distribuídos entre todos os estados $m,n$, dependentes de $A$ e $q$.

---

## Exercício 6.3

Somamos a matriz potencial $V$ à matriz cinética $H$ para obter a nova Hamiltoniana total $H_\text{total} = H + V$. A diagonalização dessa nova matriz forneceu bandas suavizadas, onde o formato e a separação entre bandas são modulados pelos parâmetros $A$ e $q$.

---

## Conclusão

Na Hamiltoniana sem potencial explícito, o parâmetro de acoplamento $\alpha$ define diretamente a abertura dos gaps de energia. Já na Hamiltoniana com potencial periódico, os parâmetros $A$ e $q$ influenciam tanto o tamanho dos gaps quanto a curvatura das bandas, resultando em uma estrutura mais distribuída e suave.
