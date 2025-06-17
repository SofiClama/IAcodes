Explicação:
O código implementa uma rede neural MLP para modelar a resposta de um circuito.
Entrada - Valores de tempo normalizados (t_norm).
Saída - Tensão normalizada (Vc_norm) do capacitor no circuito.
Arquitetura - 1 camada oculta (com 10 neurônios e ativação sigmóide) e 1 camada de saída (com 1 neurônio [sigmóide]).
Treinamento - Backpropagation (com regra delta) e função de perda (Erro quadrático médio).

1 - Por que é necessário calcular a derivada parcial?
A derivada parcial (gradiente) é usada no backpropagation para:
Ajustar os pesos  (Indica a direção e magnitude da correção necessária para minimizar o erro).
Regra da cadeia  (Permite propagar o erro das camadas de saída para as camadas ocultas).

2 - Por que usar uma função sigmóide? Por que a ReLU é mais usada?
A vantagem da sigmóide é a saída entre 0 e 1 que é útil para probabilidades ou problemas binários, já a ReLU é mais usada pois seu desempenho é superior e mais simples.
