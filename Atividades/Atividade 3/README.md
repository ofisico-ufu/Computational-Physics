# Interpolação de Funções com Redes Neurais

Neste projeto, foram desenvolvidos códigos para treinar redes neurais MLP a fim de interpolar quatro funções matemáticas: seno, tangente, sinc ($\sin(x)/x$) e gaussiana ($e^{-x^2}$) utilizando **scikit-learn**, e duas funções — sinc e gaussiana — usando **PyTorch**.

Nas implementações com scikit-learn, as redes tiveram geralmente 3 camadas ocultas com 10 neurônios por camada, exceto para a tangente que usou 12 neurônios por camada para melhor capturar sua complexidade. No PyTorch, as redes também tinham 3 camadas e 10 neurônios por camada com função de ativação tanh.

Observou-se na prática que aumentar o número de camadas e neurônios melhora a capacidade da rede de aproximar funções mais complexas, porém com custo maior em tempo de treinamento e risco de instabilidade. Para funções suaves, arquiteturas menores já são suficientes para uma boa interpolação. O projeto evidencia como a arquitetura influencia o desempenho e a precisão na regressão de funções matemáticas.

---

Além disso, foi realizado um estudo com **MLPRegressor do scikit-learn** para aprender a interpolar derivadas de funções como seno, cosseno e polinômios ($x^p$, para $p = 0$ a $10$) no intervalo de $0$ a $2\pi$.

O treinamento utilizou pontos da função como entrada e suas derivadas analíticas como saída, analisando o impacto da arquitetura da rede (número de camadas e neurônios) na capacidade de generalização e precisão da interpolação. O projeto destaca como a escolha da complexidade do modelo afeta o desempenho na regressão funcional, especialmente ao lidar com derivadas.