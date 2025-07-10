# Interpolação com Redes Neurais

Este projeto usa redes neurais para interpolar funções matemáticas com **scikit-learn** e **PyTorch**.

### Funções treinadas:

- **scikit-learn**: $\sin(x)$, $\tan(x)$, $\dfrac{\sin(x)}{x}$, $e^{-x^2}$
- **PyTorch**: $\dfrac{\sin(x)}{x}$, $e^{-x^2}$

### Arquiteturas:

- 3 camadas ocultas com 10 neurônios (12 para $\tan(x)$).
- Aumentar camadas/neurônios melhora a precisão, mas pode gerar overfitting ou instabilidade.
- Funções suaves (como $\sin(x)$) exigem menos complexidade.

---

Também treinamos redes com **MLPRegressor** para aprender **derivadas** das funções $\sin(x)$, $\cos(x)$, $\tan(x)$ e de polinômios $x^p$ ($p = 0$ a $10$), avaliando como a arquitetura da rede afeta a precisão da interpolação.