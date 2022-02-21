# Método de Simulações de Monte Carlo

## _Introdução_

O Método de Simulações de Monte Carlo (MSMC) ou somente Simulações de Monte Carlo (SMC), é uma técnica matemática muito utilizada com o intuito de medir as incertezas de eventos probabilísticos. Com isso, pode ser dito que trata-se de um conjunto de cálculos de probabilidade que mede a possibilidade de um evento futuro ocorrer.

A princípio as SMC eram mais utilizadas na solução de problemas relacionados a matemática, física e biologia. Atualmente, este método se tornou muito eficaz em áreas como finanças e investimentos, principalmente, no que tange a tomadas de decisões e como gerenciar o risco envolvido nelas.

Desta forma, a ídea desse repositório é discorrer um pouco sobre o assunto e verificar como a aplicação dessa técnica, junto com alguns conceitos da estatística, podem ajudar por exemplo na predição de ativos da bolsa de valores. 

## _Etapas Importantes Para Modelar as SMC_
O MSMC não se importa tanto com as equações diferenciais que costumam descrever sistemas mais complexos. Basicamente, o principal requisito é que o conjunto matemático e/ou físico analisado, seja modelado em função da densidade das distribuições de probabilidade (FDP).

A partir destas distribuições, a SMC deve realizar amostragem de valores aleatórios, sendo estes gerados por algoritmos matemáticos chamados de geradores de números aleatórios. Onde, os cálculos possuem uma relação com os resultados estimados anteriormente, isto é, com os dados históricos preexistentes. 

Vale ressaltar, que os resultados dos geradores não são completamente aleatórios, pois, eles possuem apenas uma aproximação de algumas propriedades destes valores, portanto eles também são denominados como números pseudo-aleatórios.

Como cada gerador possui seu próprio algoritmo de números aleatórios, é necessário informar qual será o valor inicial para fornecer os dados seguintes. Este número inicial é conhecido como semente, pois é o ponto de partida para as operações matemáticas que possibilitam a geração dos números pseudo-aleatórios. Logo, é certo dizer que cada geração de números aleatórios depende diretamente da semente utilizada.

Após, a definição da FDP e do método de geração, é realizado um processo de repetição dos valores obtidos, juntamente como alguma técnica de amostragem, esse procedimento ocorre até que os resultados esperados e/ou ponto de parada sejam atingidos.
