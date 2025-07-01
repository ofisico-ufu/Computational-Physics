## Este projeto utiliza um **MLPRegressor** do `scikit-learn` para **aprender a interpolar derivadas de funções**, explorando como a arquitetura da rede (camadas e neurônios) impacta a precisão.

* **Funções Usadas**: Seno, cosseno e polinômios ($x^p$ para $p$ de $0$ a $10$), avaliadas no domínio de $0$ a $2\pi$.
* **Dados**: Rede treinada com pontos da função como input e suas respectivas derivadas analíticas como output.
* **Análise**: Avaliação do desempenho da rede em diferentes configurações, focando na capacidade de generalização e na influência da complexidade do modelo.