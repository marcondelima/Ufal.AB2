# identificação

- Página do repositório  do trabalho ([link GitHub](https://github.com/pedrojjsantos/AB2))
- Discente 1
  - Nome : Carlos Eduardo Xavier Bezerra
  - Matrícula : 	18211739
  - Distribuição de nota (%): 33,3
- Discente 2
  - Nome : Marconde José da Silva Lima
  - Matrícula : 18211786
  - Distribuição de nota (%): 33,3
- Discente 3
  - Nome : Elygledson José da Silva Bezerra
  - Matrícula : 18211742
  - Distribuição de nota (%): 33,3

# Resultados

## Utilização intensa da UCP

*  *UCP*:

![gráfico](https://i.imgur.com/vEs0Lxm.png)

Não foi esperado, acreditavamos que o consumo da unidade central de processamento seria totalmente crescente, o que não ocorreu a partir do sétimo segundo.

## Utilização intensa da UCP e memória

*  *Memória e UCP*:

O lado esquerdo representa o uso em porcentagem da UCP, enquanto o lado direito sendo representado também por porcentagem, é baseado no valor de 10 gigabytes como valor total. 

![gráfico](https://i.imgur.com/fOdk8BB.png)

Em relação aos resultados do nosso programa , em sua maioria, eles cumpriram com nossas expetativas. Os testes realizados na Unidade Central de Processamento através do comando ./bin ucp, atingiram altos níveis de consumo fazendo, os dispositivos utilizados nos testes,  apresentarem lerdeza ao executar determinados processos. Por outro lado, os testes realizados na memória, cumpriram em parte com nossas expectativas, utilizamos primeiramente uma função chamada usleep(), cuja função é atrasar a execução do programa em milionésimos de segundo, para limitar o uso do malloc(),  função essa que possibilita uma alocação dinâmica na memória RAM, e ao fazer isso tanto o uso da UCP, quanto da memória não atingiram altos níveis, portanto, durante o tempo de execução do programa, foi possível realizar tarefas sem nenhum problema. Em contrapartida, ao retirar a função usleep(), tanto o consumo de UCP, quanto de memória atingiram altíssimos níveis de consumo, causando extrema lentidão e até travamento dos dispositivos. Com base nisso, durante a execução do programa, notamos alguns pontos importantes a respeito da função usleep(), a qual independente do valor acrescentado na função malloc(), pois com ela ativada tanto o consumo de memória como o de UCP são baixos. 

Um dos computadores utilizados no processo de testes possuía um processador core i5, com 8GB de memória. Nesse dispositivo,  um caso interessante aconteceu enquanto testávamos  o programa sem a função usleep(). Durante a execução, tanto o consumo de UCP quanto o consumo da memória abaixaram rapidamente até chegar a zero, faltando poucos segundos para o programa terminar sua execução.

![gráfico](https://i.imgur.com/MrjXais.png)

Após outros testes, o mesmo caso se repetiu, no entanto, dessa vez apenas o consumo de UCP que abaixou bruscamente, enquanto o nível de consumo da memória se manteve até o final da execução.

![gráfico](https://i.imgur.com/bglHKpX.png)


