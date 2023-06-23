# Método de Condorcet
O Método de Condorcet é uma técnica de decisão que busca encontrar uma alternativa preferida a partir de comparações diretas entre as alternativas disponíveis. Ele é baseado na ideia de que se uma alternativa for preferida em relação a todas as outras emparelhadas individualmente, então ela deve ser a escolha preferida em relação ao conjunto completo de alternativas.

Neste repositório, apresento um código em Python que implementa o Método de Condorcet para um determinado conjunto de alternativas e critérios de classificação. O código utiliza a biblioteca Pandas para armazenar e manipular os dados.
## Como usar o código
1. O usuário deve executar o código Python fornecido.<br/>
2. Será solicitado que o usuário insira o número de alternativas desejadas e, em seguida, digite o nome de cada alternativa.<br/>
3. Em seguida, o usuário deve inserir o número de critérios desejados e fornecer o nome de cada critério.<br/>
4. Para cada critério, o usuário será solicitado a classificar cada alternativa de acordo com uma escala pré-definida.<br/>
5. O código irá gerar uma tabela de classificações, mostrando as classificações dadas pelo usuário para cada critério e alternativa.<br/>
6. Em seguida, o código calculará as matrizes de comparação para cada critério, seguindo as regras do Método de Condorcet.<br/>
7. Serão exibidas as matrizes de comparação para cada critério.<br/>
8. O código somará as matrizes de cada critério para formar uma matriz de decisão.<br/>
9. A matriz de decisão será processada de acordo com as regras do Método de Condorcet, atribuindo valores (+1, 0 ou -1) para cada par de alternativas.<br/>
10. Será exibida a matriz de decisão resultante.<br/>
11. O código determinará a posição de cada alternativa com base no número de sinais positivos na matriz de decisão.<br/>
12. O resultado do método será exibido, mostrando a ordem de classificação das alternativas.
## Requisitos
- Python 3.x<br/>
- Biblioteca Pandas
## Exemplo
Aqui está um exemplo de execução do código:<br/>
Quantas alternativas você deseja inserir? 3<br/>
Digite a alternativa 1: A<br/>
Digite a alternativa 2: B<br/>
Digite a alternativa 3: C<br/>

Quantos critérios você deseja inserir? 2<br/>
Digite o critério 1: C1<br/>
Digite o critério 2: C2<br/>

Classifique cada alternativa de acordo com a escala abaixo:<br/>
5- Muito Bom<br/>
4- Bom<br/>
3- Neutro<br/>
2- Ruim<br/>
1 - Muito ruim<br/>

Classificação para o critério C1<br/>
Digite a classificação para a alternativa A: 4<br/>
Digite a classificação para a alternativa B: 5<br/>
Digite a classificação para a alternativa C: 3<br/>

Classificação para o critério C2<br/>
Digite a classificação para a alternativa A: 2<br/>
Digite a classificação para a alternativa B: 4<br/>
Digite a classificação para a alternativa C: 5<br/>

Tabela de Classificações:<br/>

   C1  C2<br/>
A   4   2<br/>
B   5   4<br/>
C    3   5<br/>

Matriz para o critério 'C1':<br/>
[0, -1, 1]<br/>
[1, 0, 1]<br/>
[-1, -1, 0]<br/>

Matriz para o critério 'C2':<br/>
[0, -1, 1]<br/>
[1, 0, 1]<br/>
[-1, -1, 0]<br/>

Matriz de Decisão:<br/>
[0, -2, 2]<br/>
[2, 0, 2]<br/>
[-2, -2, 0]<br/>

Resultado do método:<br/>
1º lugar: B<br/>
2º lugar: A<br/>
3º lugar: C
## Considerações Finais
O Método de Condorcet oferece uma abordagem interessante para tomar decisões com base em comparações diretas entre alternativas. No entanto, é importante considerar as limitações e premissas associadas a esse método. Certifique-se de entender as características e o contexto específico do problema que está sendo resolvido antes de aplicar o Método de Condorcet ou qualquer outro método de decisão
