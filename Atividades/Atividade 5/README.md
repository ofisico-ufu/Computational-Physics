# Exercícios - Diagrama de Bandas com Hamiltonianas Periódicas

## Exercício 6.1

Construímos uma matriz Hamiltoniana $5 \times 5$ para calcular o diagrama de bandas. A matriz foi diagonalizada com termos da forma:

- Diagonal principal: $H_{ii} = (k - 2\pi n_i)^2$
- Acoplamentos: $H_{0,4} = H_{4,0} = 2.0$ (entre $n = \pm2$) e $H_{1,3} = H_{3,1} = 2.0$ (entre $n = \pm1$)
- Os demais termos foram definidos como zero.

## Exercício 6.2

Calculamos os coeficientes de uma matriz potencial $V_{5 \times 5}$ com amplitude $A = 3$ e frequência $q = 0{,}5$, utilizando a expressão:

$$
V_{m,n} = \int_0^1 A \cos(2\pi q x) \cdot e^{i 2\pi (m-n)x} \, dx
$$

## Exercício 6.3

Obtivemos uma nova Hamiltoniana total somando $H + V$, e recalculamos o diagrama de bandas com os novos termos.

---

Na Hamiltoniana com potencial nulo, o valor do acoplamento $\alpha$ determina diretamente o tamanho do gap de energia. Já na Hamiltoniana com potencial periódico, o tamanho e a suavidade das bandas dependem dos parâmetros $A$ e $q$, afetando a curvatura e a abertura dos gaps de forma mais distribuída.