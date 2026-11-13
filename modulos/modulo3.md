---
title: A matemática da ruína do apostador - probabilidade e esperança matemática
subject: Módulo 3
---

```{important} Objetivo
O objetivo deste modulo é utilizar tabelas juntamente com o conceito matemático, proporcionando ao aluno entender o conceito de Esperança matemática negativa sem se apegar de início com excesso às fórmulas complexas do conteúdo, desconstruindo a ideia de sorte e que consequentemente apostas levam à liquidação do patrimônio financeiro.
```

## Desmistificando a sorte através da probabilidade

No dia a dia, dizemos que sorte é uma palavra utilizada para justificar eventos que não podemos prever, ou seja, imprevisíveis. Entretanto, quando falamos em jogos de azar, sorte é quantificável e tem um nome: *probabilidade*. A compreensão das probabilidades envolvidas nos jogos de azar permite analisar matematicamente situações que, no senso comum, costumam ser associadas exclusivamente à sorte [@moscardini2025jogos]. Na Matemática, a probabilidade de um evento $A$ é representada por $P(A)$. Considerando um espaço amostral finito $\Omega$, no qual todos os resultados elementares são igualmente prováveis, a probabilidade de ocorrência de um evento pode ser calculada pela razão entre o número de resultados favoráveis e o número total de resultados possíveis. Assim, temos:

```{math}
:name: eq:probabilidade
P(A) = \frac{|A|}{|\Omega|},
```
em que $A$ representa o evento considerado, $|A|$ corresponde ao número de resultados favoráveis à sua ocorrência e $|\Omega|$ representa o número total de resultados possíveis. Essa expressão corresponde à definição clássica de probabilidade e pressupõe que todos os resultados elementares sejam equiprováveis. Quando essa condição não é satisfeita, a probabilidade deve ser determinada considerando as probabilidades associadas aos diferentes resultados.

Considerando um dado equilibrado de seis faces, no qual todos os resultados possuem a mesma probabilidade de ocorrência, a probabilidade de obter o número 5 em um lançamento é de 1/6, aproximadamente 16,7%. O dado não tem uma memória, ou seja, se o número 5 saiu três vezes seguidas, a chance de ele sair em uma quarta jogada continua sendo a mesma, 1/6, pois os eventos são independentes. Em jogos de apostas, a combinação entre as probabilidades dos resultados e os valores financeiros associados a eles pode estabelecer uma vantagem matemática para a banca. Quando a esperança matemática do resultado líquido do apostador é negativa, existe uma perda média esperada por jogada. Entretanto, isso não significa que todas as apostas resultarão em prejuízo, pois ganhos individuais podem ocorrer, embora a repetição do jogo, sob condições apropriadas, apresente uma tendência média desfavorável ao apostador.


## Esperança matemática e o porquê de a banca sempre ganhar

A esperança matemática, denotada por $E[X]$, representa o valor médio esperado dos resultados de uma variável aleatória $X$, que, neste contexto, corresponde ao resultado financeiro líquido de uma jogada. Com base no valor da esperança matemática, um jogo pode ser classificado como:

* **Justo**, se $E[X] = 0$, não apresentando ganho ou perda média esperada por jogada.
* **Favorável**, se $E[X] > 0$, indicando um resultado financeiro médio esperado positivo.
* **Desfavorável (ou ruína)**, se $E[X] < 0$, indicando um resultado financeiro médio esperado negativo, sem que isso implique necessariamente a perda integral do patrimônio.

Um exemplo prático, seria imaginar um jogo de cara ou coroa com uma moeda modificada.
Suponha que um amigo te chame para jogar cara ou coroa.
A probabilidade de dar cara é de 50%, assim como dar coroa é de 50%.

* Se der cara, você ganha R\$ 10,00 (dez reais);
* Se der coroa, você perde R\$ 12,00 (doze reais).

Calculando a esperança matemática deste jogo, temos:

:::{math}
E[X] = (10 \times 0{,}5) + (-12 \times 0{,}5) = 5 - 6 = -1
:::

A interpretação da situação acima significa que, a cada jogada, você tem uma possibilidade média de perder R\$ 1,00 (um real). Se você jogar uma única vez, você pode ter a sorte de sair cara e ganhar R\$ 10,00 (dez reais). Considere que esse mesmo jogo seja repetido mil vezes, mantendo-se as probabilidades e os valores de ganho e perda estabelecidos no exemplo, e admitindo-se que as jogadas sejam independentes. Como a esperança matemática é de -R\$ 1,00 por jogada, a perda total esperada após mil repetições será de R\$ 1.000,00. Entretanto, esse valor representa uma expectativa matemática, e não um prejuízo necessariamente observado em todas as sequências de mil jogadas. Os resultados efetivos poderão apresentar variações, inclusive com ganhos em determinadas trajetórias. O exemplo constitui um modelo didático simplificado de um jogo com esperança matemática negativa, não representando necessariamente as probabilidades e os pagamentos específicos de cada plataforma de apostas.

## Laboratório Computacional - é hora de simular a Lei dos Grandes Números

```{important} Objetivo da atividade
Utilizar planilhas eletrônicas, como Microsoft Excel ou Google Sheets, para simular sequências de apostas com esperança matemática negativa, possibilitando a observação da variabilidade dos resultados acumulados e a investigação da relação entre o comportamento médio das simulações e o valor esperado previsto pelo modelo probabilístico.
```

Diferentemente do exemplo anterior, no qual se considerou um jogo de cara ou coroa com probabilidades iguais de 50% e pagamentos assimétricos de R\$ 10,00 e R\$ 12,00, a presente simulação utiliza um modelo com probabilidades distintas de ganho e perda. Nesse segundo cenário, considera-se uma probabilidade de 45% para o ganho de uma unidade monetária e de 55% para a perda de uma unidade monetária. A utilização desses dois modelos tem finalidade didática, permitindo compreender que a esperança matemática depende tanto das probabilidades dos resultados quanto dos valores financeiros associados a eles.

Nesta atividade, o saldo acumulado corresponde à soma algébrica dos ganhos e perdas registrados ao longo das jogadas simuladas. Considerando $X_k$ como o resultado líquido da $k$-ésima jogada, esse saldo é representado por $S_n = \sum_{k=1}^{n} X_k$. O modelo admite resultados acumulados negativos, pois não estabelece um capital financeiro inicial nem uma condição de interrupção das apostas. Dessa forma, a planilha permite investigar o comportamento dos resultados aleatórios e sua relação com a esperança matemática, mas não representa diretamente o patrimônio disponível de um apostador nem constitui um modelo de ruína financeira.

### Roteiro

1. Leve os alunos para o laboratório de informática da escola, ou previamente solicite que os alunos levem para escola, dispositivos que permitam a utilização de aplicativos de planilhas eletrônicas (celulares ou *tablets*).
2. Oriente a construção de uma planilha que simule o segundo modelo probabilístico apresentado, considerando uma probabilidade de ganho de 45% e uma probabilidade de perda de 55%, com resultados financeiros líquidos de uma unidade monetária positiva ou negativa por jogada.
    - Na Célula `A1`, peça que escrevam: `Jogada`; Na Célula `B1`: `Resultado`; e na Célula `C1`: `Saldo Acumulado`
    - Na Célula `A2`, peça que coloque o número `1`, e na Célula `A3` o número `2`, em seguida peça que selecione as duas e arraste até obter o valor `500`, que será na Célula `A501`.
    - Na Célula `B2`, utilize uma das funções: `=SE(ALEATÓRIO()<=0,45; 1; -1)` ou `=SE(ALEATÓRIOENTRE(1;100)<=45; 1; -1)`, e peça que arraste até a Célula `B501`. Aqui o resultado será `1` ou `-1`, definindo se o apostador na jogada ganhou ou perdeu, respectivamente.
    - Na Célula `C2`, insira a fórmula `=B2`, que representa o resultado acumulado após a primeira jogada. Em seguida, na Célula `C3`, insira a fórmula `=C2+B3`, que adiciona ao saldo anterior o resultado da jogada seguinte. Selecione a Célula `C3` e arraste a fórmula até a Célula `C501`, correspondente à 500ª jogada. Dessa maneira, a coluna `C` apresentará, a cada linha, a soma acumulada dos ganhos e das perdas obtidos na simulação.
3. Solicite que os alunos façam uma análise gráfica, ao pedir que selecionem a coluna do saldo acumulado (Coluna `C`), e indo na aba `Inserir` do menu principal, clicar em `Gráfico`.
O resultado final da planilha deve ser parecido com:

```{image} m3-planilha.png
:alt: Ilustração da planilha elaborada pelos alunos no Módulo 3
:width: 500px
:align: center
```

4. Os alunos observarão que em um curto prazo, até a jogada 20 ou 30, o gráfico oscilará muito. Alguns alunos terão linhas crescentes, o que indica lucro temporário, gerando a falsa sensação de que estão ganhando. Mas em um longo prazo, será perceptível que praticamente todos os gráficos da sala apontarão para valores negativos. No geral, a linha do início ao fim representará uma ordem decrescente. Ao comparar os gráficos produzidos, os estudantes poderão observar trajetórias distintas, incluindo períodos de ganhos e de perdas. Como o modelo apresenta esperança matemática negativa, é esperado que o resultado acumulado apresente tendência decrescente em termos médios, embora uma simulação individual possa registrar oscilações significativas e até terminar com saldo positivo. O professor deverá incentivar a comparação entre diferentes trajetórias e discutir a diferença entre os resultados observados e o comportamento esperado teoricamente.

```{attention} Importante
A Lei dos Grandes Números estabelece que, sob hipóteses apropriadas, a média dos resultados de um grande número de repetições tende à esperança matemática da variável aleatória considerada. Assim, em um jogo com esperança negativa, a média dos ganhos líquidos por jogada tende a um valor negativo, ainda que os resultados acumulados de diferentes simulações apresentem oscilações. A convergência da média não significa que todas as trajetórias apresentarão exatamente o prejuízo esperado.
```