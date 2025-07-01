O código apresentado no artigo é sobre o DBSCAN com o uso de Python.


O que é DBSCAN?

O DBSCAN é um algoritmo de agrupamento baseado em densidade. Ele agrupa pontos que estão próximos uns dos outros (alta densidade) e marca pontos em áreas de baixa densidade como outliers (ruído).


Como o algoritmo funciona?

Primeiro o DBSCAN começa escolhendo um ponto aleatório que ainda não foi visitado. Em seguida, busca por vizinhos e encontra todos os pontos dentro do raio, se o número de vizinhos for maior ou igual ao parâmetro "min_samples", forma um novo cluster. Por fim, pontos que não pertencem a nenhum cluster são marcados como -1.
