---
title: A matemática da acumulação - Juros Compostos e Progressão Geométrica
subject: Módulo 4
---

```{important} Objetivo
O objetivo deste modulo é novamente utilizar tabelas juntamente com o conceito matemático, mas agora proporcionando ao aluno entender o conceito de Juros Compostos, ou seja, fazendo um contraponto em relação ao módulo anterior ao mostrar como o tempo e a matemática da progressão geométrica dos juros compostos trabalham a favor do investidor, em uma aplicação financeira como a renda fixa, por exemplo, e que consequentemente levará a acumulação do patrimônio financeiro.
```
## O poder do tempo, do crescimento linear ao exponencial

Quando trabalhamos, ao receber o nosso salário, sempre nos deparamos com determinadas demandas a cumprir como forma de custear as necessidades mensais de consumo (água, luz, internet, feira, ...). Sempre que sobra um pouquinho no final, o ideal é guardar, e a organização das receitas, despesas, poupança e planejamento constitui elemento importante para uma gestão consciente dos recursos financeiros [@bcb2026caderno]. Mas guardar, apenas por guardar não apresenta muita vantagem, pois em regra, se a cada mês você guarda um valor, esse será somado ao do próximo, e assim sucessivamente, gerando um crescimento patrimonial. E se esse valor for fixo, ou seja, todos os meses sobra o mesmo valor para ser guardado, em regra temos um crescimento linear de recursos, onde o patrimônio vai crescer sempre o mesmo valor. Nesse caso, o melhor é utilizar a lógica do crescimento exponencial presente no universo dos investimentos.

A diferença entre os dois modelos é percebida ao comparar dois conceitos matemáticos, a Progressão Aritmética (PA) e a Progressão Geométrica (PG) [@assafneto2021matematica]:

- Na PA, sob o viés dos investimentos financeiros, temos que tratá-la como juros simples, onde o rendimento é calculado sempre sobre o valor inicial depositado. Nesse caso o crescimento é linear e, portanto, previsível em uma linha reta.

- Na PG, sob o viés dos investimentos financeiros, temos que tratá-la como juros compostos, onde o rendimento de cada período é adicionado ao capital para a render no período seguinte. Nesse caso o crescimento é exponencial e, portanto, previsível em uma curva exponencial.

No início de uma aplicação financeira, a diferença entre esses crescimentos, linear e exponencial, é quase imperceptível, podendo ser até desconsiderado. Entretanto, à medida que o tempo avança, a curva exponencial se inclina para cima de forma acentuada, afastando-se da linha reta. Tal fato, multiplica o patrimônio de forma segura e duradoura, e de uma maneira muito mais significativa em detrimento de buscar os atalhos da sorte em jogos de azar.

## Modelagem matemática da formação de um patrimônio

Ao guardarmos aquele dinheiro que sobra ao final de um mês em um espaço de tempo, devemos levar em consideração que o desejo é de que esse dinheiro atinja o maior crescimento possível, ou seja, que cresça exponencialmente. Em uma aplicação financeira, cujo sistema de rendimento é assim definido, temos que calcular o montante acumulado por meio dos aportes mensais, considerando que estes sejam valores constantes, ao longo do espaço de tempo. Para isso, utilizamos a fórmula da soma dos termos de uma PG finita com uma adaptação à matemática financeira dos juros compostos: 

$$
M = P \cdot \frac{(1 + i)^n - 1}{i}
$$

onde:
- $M$ é o montante final acumulado;
- $P$ é o valor do Aporte Periódico (mensal);
- $i$ é a taxa de juros por período (mensal);
- $n$ é o número total de período (meses).

Veja que com $n$ no expoente, quanto maior for o valor dele, maior será o montante final acumulado $M$, ou seja, o tempo é fator determinante para que o ativo financeiro seja tão grande e representativo quanto queira. E daí, podemos dizer que quanto antes se começa a investir pequenas quantias poupadas de forma constante no início da vida, o resultado será significativamente maior do que investido tardiamente.

## Atividade Investigativa: O laboratório do futuro

```{important} Objetivo da atividade
Construir uma planilha comparativa para investigar a diferença entre guardar o dinheiro de forma parada (sem rendimento) e investindo em um regime de juros compostos. Tornando clara a interpretação de que no investimento em uma renda fixa com aportes mensais o patrimônio sempre será positivo e que atrelado ao tempo o seu crescimento é exponencialmente satisfatório. 
```

### Roteiro

1. Leve os alunos para o laboratório de informática da escola, ou previamente solicite que os alunos levem para escola, dispositivos que permitam a utilização de aplicativos de planilhas eletrônicas (Celulares ou Tablets). 
2. Apresente a seguinte situação aos alunos:
    - "Se você conseguisse poupar R$ 50,00 por mês, de tudo que você recebe no mês (como mesada por exemplo), qual seria o valor acumulado ao longo de 1 ano, 5 anos e 10 anos?" 
3. Oriente a construção das planilhas, pedindo que os alunos criem uma tabela que simule essa situação:
    - Na Célula `A1`, peça que escrevam: `Tempo (meses)`; Na Célula `B1`: `Acumulado (sem rendimento)`; na Célula `C1`: `Acumulado (juros compostos)`.
    - Na Célula `A2`, peça que coloquem o número `1`, e na Célula `A3` o número `2`, em seguida peça que selecione as duas e arraste até o valor `120` que será na Célula `A121`.
    - Na Célula `B2`, peça que coloquem a função: `=50*A2`, e em seguida arrastar até a célula `B121`. Aqui o aluno verá que com 1 ano (12 meses), 5 anos (60 meses) e 10 anos (120 meses), o acúmulo nada mais é que a soma apenas dos aportes mensais fixos até determinado ponto de análise.
    - Na Célula `C2`, peça que coloquem a função: `=VF(0,8%; A2; -50; 0; 0)`, e em seguida arrastar até a célula `C121`. Aqui o aluno verá que com 1 ano (12 meses), 5 anos (60 meses) e 10 anos (120 meses), o acúmulo representará um valor futuro acumulado, gerado pela soma dos aportes mensais fixos com os rendimentos de cada um deles até determinado ponto de análise.
4. Solicite que os alunos façam uma análise gráfica, ao pedir que selecionem as três colunas, e indo na aba inserir, gráficos recomendados, e clicar na segunda opção de gráfico de linhas recomendada. O resultado deve ser parecido com o seguinte:

```{image} m4-planilha.png
:alt: Ilustração da planilha elaborada pelos alunos no Módulo 4
:width: 500px
:align: center
```

5. Desafie os alunos para que digam em que momento (mês/ano) a distância entre a linha do acúmulo simples e a linha do acúmulo nos juros compostos começa a se tornar evidente. 

6. Os alunos concluirão que, em se tratando de poupar dinheiro, é mais válido guardar em uma aplicação de renda fixa no regime de juros compostos, e que quanto antes eles façam isso, mais o tempo será parceiro deles na objetivação do patrimônio financeiro que se deseja alcançar.

```{attention} Importante
A atividade expõe que pela modelagem matemática de aportes constantes mensais em uma aplicação financeira de renda fixa, quanto maior for o valor desses aportes aliado à quanto maior for o tempo/período em que a aplicação ficará vigente, o crescimento do patrimônio financeiro cresce exponencialmente. E isso ocorre independentemente de considerar outros fatores econômicos no período, como taxas, inflação, etc.
```