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

Após, a definição da FDP e do método de geração, é realizado um processo de repetição dos valores obtidos, juntamente como alguma técnica de amostragem, esse procedimento ocorre até que os resultados esperados e/ou ponto de parada sejam atingidos. Veja uma ilustração simplificada de um processo de simulação.

   ![image](https://user-images.githubusercontent.com/31603707/154871246-8e9db8a3-f407-4291-bc82-38ad840bc6fe.png?)

## Modelo 1: Aplicando Simulações de Monte Carlo para estimar o valor de π

Para comprovar que o método funciona e facilitar o entendimento do processo das SMC, modelei uma FDP para estimar o valor da constante de π, pois, este é um dado bastante conhecido. Para ver as definições utilizadas na modelagem da função verifique o arquivo Jupyter Notebook <a href="https://github.com/luanjesus/metodo-simulacao-monte-carlo/blob/main/estimando_valor_pi_smc.ipynb">estimando_valor_pi_smc.ipynb</a>.

Neste processo, foram geradas algumas simulações com os valores 10, 100, 1000, 10000 e 100000, conforme o número ia aumentando o valor estimado se aproximava bastante do resultado esperado (3,14). Sendo que acima de 1000 repetições a taxa de acerto já era superior a 96%, ou seja, os valores eram bem próximos do resultado real.

- **Resultados obtidos na Simulação 1**

    ![image](https://user-images.githubusercontent.com/31603707/154872701-6027c6ee-0a7d-448c-87c6-e30aba31bc28.png)

- **Resultados obtidos na Simulação 2**

    ![image](https://user-images.githubusercontent.com/31603707/154873242-5d061fab-7224-4530-a87f-6b21786b29a1.png)

- **Gráfico Scatter com a distribuição dos pontos gerados nas simulações**

    ![image](https://user-images.githubusercontent.com/31603707/154873754-a9fc8249-e54b-4716-8dc9-1aed247d7db6.png)



