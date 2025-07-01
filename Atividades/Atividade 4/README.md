#Esta atividade teve como objetivo resolver a EDO do resfriamento de uma caneca de café, comparando abordagens analítica, numérica e baseadas em redes neurais, incluindo PINNs (Physics-Informed Neural Networks).

A equação diferencial considerada foi:

\[
\frac{dT}{dt} = r(T_{\text{amb}} - T), \quad T_{\text{amb}} = 25^\circ C, \quad r = 0{,}005 \, \text{s}^{-1}
\]

## Etapas Realizadas

### 1. Solução Analítica
Resolvi a EDO analiticamente para obter a função exata da temperatura em função do tempo.

### 2. Solução Numérica (RK4)
Implementei a solução numérica da EDO utilizando `scipy.integrate.solve_ivp` (método RK4) e comparei com a solução analítica.

### 3. Geração de Dados Sintéticos
Utilizei a solução analítica para gerar 10 pontos com ruído gaussiano (média 0, desvio padrão 0.5) no intervalo de 0 a 200 s para simular dados experimentais.

### 4. Regressão com Rede Neural Simples
Treinei uma rede neural de regressão com os dados sintéticos e testei a extrapolação até 1000 s. Como esperado, a extrapolação foi ineficaz.

### 5. PINN com r conhecido
Implementei uma PINN incorporando o valor conhecido de \( r = 0{,}005 \, \text{s}^{-1} \) na função de perda. A rede foi treinada com os dados sintéticos e obteve bom desempenho em comparação com a solução analítica.

### 6. PINN com r desconhecido
Treinei uma nova PINN assumindo \( r \) desconhecido. A rede foi capaz de estimar o valor de \( r \) com precisão e produzir resultados consistentes com a solução analítica.