---
title: A matemática da ruína do apostador - probabilidade e esperança matemática
subject: Módulo 3
---

```{important} Objetivo
O objetivo deste modulo é utilizar tabelas juntamente com o conceito matemático, proporcionando ao aluno entender o conceito de Esperança matemática negativa sem se apegar de início com excesso às fórmulas complexas do conteúdo, desconstruindo a ideia de sorte e que consequentemente apostas levam à liquidação do patrimônio financeiro.
```

## Desmistificando a sorte através da probabilidade

No dia a dia, dizemos que sorte é uma palavra utilizada para justificar eventos que não podemos prever, ou seja, imprevisíveis. Entretanto, quando falamos em jogos de azar, sorte é quantificável e tem um nome: *probabilidade*. A compreensão das probabilidades envolvidas nos jogos de azar permite analisar matematicamente situações que, no senso comum, costumam ser associadas exclusivamente à sorte [@moscardini2025jogos]. Na matemática, a probabilidade é a chance de um determinado evento ocorrer através de uma razão entre o número de casos favoráveis e o número total de casos possíveis:

```{math}
:name: eq:probabilidade
P(X) = \frac{\text{n}^{\underline{\text{o}}} \text{ de casos favoráveis}}{\text{n}^{\underline{\text{o}}} \text{ de casos possíveis}}
```

Usando um dado comum de 6 faces como exemplo, a chance de sortear o número 5 é de 1/6 (aproximadamente 16,7%). O dado não tem uma memória, ou seja, se o número 5 saiu três vezes seguidas, a chance dele sair em uma quarta jogada continua sendo a mesma, 1/6, pois os eventos são *independentes*. Já as plataformas de apostas, apesar de utilizar essa mesma lógica de eventos, elas ajustam as regras de tal forma que a soma de todas as probabilidades de ganho do apostador não supere, de forma alguma, a vantagem da casa de aposta, ou seja, o apostador sempre perde e as plataformas sempre ganham.

## Esperança matemática e o porquê de a banca sempre ganhar

O que garante o lucro das casas de apostas, e consequentemente, a ruína financeira do apostador no longo prazo, é o conceito da *esperança matemática*, denotada por $E[X]$. Trata-se da representação do valor médio esperado de ganho ou perda em um cenário de repetição de jogadas. Com a esperança matemática, dizemos que um jogo é:

* **Justo**, se $E[X] = 0$, ou seja, no longo prazo, ninguém perde e ninguém ganha.
* **Favorável**, se $E[X] > 0$, ou seja, no longo prazo, o jogador tende a lucrar.
* **Desfavorável (ou ruína)**, se $E[X] < 0$, ou seja, no longo prazo o jogador inevitavelmente perderá todo o seu dinheiro.

Um exemplo prático, seria imaginar um jogo de cara ou coroa com uma moeda modificada.
Suponha que um amigo te chame para jogar cara ou coroa.
A probabilidade de dar cara é de 50%, assim como dar coroa é de 50%.

* Se der cara, você ganha R\$ 10,00 (dez reais);
* Se der coroa, você perde R\$ 12,00 (doze reais).

Calculando a esperança matemática deste jogo, temos:

:::{math}
E[X] = (10 \times 0{,}5) + (-12 \times 0{,}5) = 5 - 6 = -1
:::

A interpretação da situação acima significa que, a cada jogada, você tem uma possibilidade média de perder R\$ 1,00 (um real). Se você jogar uma única vez, você pode ter a sorte de sair cara e ganhar R\$ 10,00 (dez reais). Mas se você jogar, por exemplo, 1000 vezes, a matemática vai se impor e você terminará com um prejuízo próximo de R\$ 1000,00 (mil reais). As *bets* e o jogo do tigrinho funcionam assim.

## Laboratório Computacional - é hora de simular a Lei dos Grandes Números

```{important} Objetivo da atividade
Utilizar uma planilha eletrônica (Excel ou Google Sheets) na simulação do comportamento de um jogador após centenas de apostas, e identificando que o patrimônio converge para a perda total.
```

### Roteiro

1. Leve os alunos para o laboratório de informática da escola, ou previamente solicite que os alunos levem para escola, dispositivos que permitam a utilização de aplicativos de planilhas eletrônicas (celulares ou *tablets*).
2. Oriente a construção das planilhas, pedindo que os alunos criem uma tabela que simule o jogo da moeda modificado (ou um modelo onde a chance de ganho é de 45% e a de perda é de 55%, como parâmetros hipotéticos do modelo didático).
    - Na Célula `A1`, peça que escrevam: `Jogada`; Na Célula `B1`: `Resultado`; e na Célula `C1`: `Saldo Acumulado`
    - Na Célula `A2`, peça que coloque o número `1`, e na Célula `A3` o número `2`, em seguida peça que selecione as duas e arraste até obter o valor `500`, que será na Célula `A501`.
    - Na Célula `B2`, utilize uma das funções: `=SE(ALEATÓRIO()<=0,45; 1; -1)` ou `=SE(ALEATÓRIOENTRE(1;100)<=45; 1; -1)`, e peça que arraste até a Célula `B501`. Aqui o resultado será `1` ou `-1`, definindo se o apostador na jogada ganhou ou perdeu, respectivamente.
    - Na Célula `C3`, utilize `=B2`, na Célula `C4`, utilize `=C2+B3`, e peça que arrastem até a célula `C501`. Aqui será realizado o cálculo do saldo atual somando ou subtraindo o valor do resultado da jogada anterior.
3. Solicite que os alunos façam uma análise gráfica, ao pedir que selecionem a coluna do saldo acumulado (Coluna `C`), e indo na aba `Inserir` do menu principal, clicar em `Gráfico`.
O resultado final da planilha deve ser parecido com:

```{image} m3-planilha.png
:alt: Ilustração da planilha elaborada pelos alunos no Módulo 3
:width: 500px
:align: center
```

4. Os alunos observarão que em um curto prazo, até a jogada 20 ou 30, o gráfico oscilará muito. Alguns alunos terão linhas crescentes, o que indica lucro temporário, gerando a falsa sensação de que estão ganhando. Mas em um longo prazo, será perceptível que praticamente todos os gráficos da sala apontarão para valores negativos. No geral, a linha do início ao fim representará uma ordem decrescente.

```{attention} Importante
A atividade demonstra visualmente que pela Lei dos Grandes Números, quanto maior for a quantidade de repetições em um jogo de esperança matemática negativa, mais o resultado se aproximará da perda prevista pela teoria.
```