## Esta atividade teve como objetivo resolver a EDO do resfriamento de uma caneca de café, comparando abordagens analítica, numérica e baseadas em redes neurais, incluindo PINNs (Physics-Informed Neural Networks).

A equação diferencial considerada foi:

$$
\frac{dT}{dt} = r(T_{\text{amb}} - T), \quad T_{\text{amb}} = 25^\circ C, \quad r = 0.005 \ \text{s}^{-1}
$$

## Etapas Realizadas

### 1. Solução Analítica
Resolvi a EDO analiticamente para obter a função exata da temperatura em função do tempo.

### 2. Solução Numérica (RK4)
Implementei a solução numérica usando `scipy.integrate.solve_ivp` (método de Runge-Kutta de 4ª ordem) e comparei com a solução analítica.

### 3. Geração de Dados Sintéticos
Gerei 10 pontos com base na solução analítica no intervalo de 0 a 200 s, adicionando ruído gaussiano com média 0 e desvio padrão 0.5.

### 4. Regressão com Rede Neural Simples
Treinei uma rede neural de regressão com os dados sintéticos e avaliei a extrapolação até 1000 s. A extrapolação foi imprecisa, como esperado.

### 5. PINN com $r$ conhecido
Implementei uma PINN informada pela física, assumindo o valor conhecido de $r = 0.005$. A rede apresentou resultados próximos da solução analítica.

### 6. PINN com $r$ desconhecido
Treinei uma nova PINN sem conhecer $r$. A rede estimou corretamente o valor de $r$ e replicou bem a dinâmica da solução analítica.
