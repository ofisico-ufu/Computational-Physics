# Projeto de Interpolação com Redes Neurais

Foi desenvolvido um conjunto de códigos utilizando redes neurais para treinar e interpolar as funções $\sin(x)$, $\tan(x)$, $\text{sinc}(x) = \frac{\sin(x)}{x}$ e $e^{-x^2}$, empregando as bibliotecas **scikit-learn** e **PyTorch**. No scikit-learn, as quatro funções foram abordadas, enquanto no PyTorch focamos em duas delas: $\text{sinc}(x)$ e $e^{-x^2}$.

Nas implementações, foram usadas redes com 3 camadas ocultas e 10 neurônios por camada, exceto para $\tan(x)$, que exigiu 12 neurônios por camada devido à sua maior complexidade. Observou-se que, ao aumentar o número de camadas e neurônios, a rede melhora a capacidade de interpolar funções complexas, mas pode aumentar o tempo de treinamento e o risco de instabilidade. Funções mais suaves, como $\sin(x)$, podem ser bem aproximadas com arquiteturas menores.

Além disso, realizamos treinamentos com o **MLPRegressor** do scikit-learn para aprender a interpolar as derivadas de funções trigonométricas, incluindo $\sin(x)$, $\cos(x)$ e $\tan(x)$. Nesse estudo, exploramos como a arquitetura da rede — número de camadas e neurônios — impacta a precisão da interpolação das derivadas.
