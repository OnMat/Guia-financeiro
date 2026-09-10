---
title: Manual do Professor
subject: Módulo 6
---

```{important} Objetivo
O objetivo deste módulo é ofertar a você professor, orientações didáticas para a devida aplicação da sequência didática proposta neste guia. São disponibilizadas sugestões metodológicas, respostas esperadas para as atividades investigativas, observações pedagógicas, bem como materiais complementares que vão auxiliar na condução das discussões, bem como na utilização das planilhas eletrônicas. É importante ressaltar, que as respostas apresentadas aqui são de caráter orientador, não sendo, portanto, únicas, uma vez que diferentes estratégias e argumentos matemáticos devem surgir durante as investigações por parte dos estudantes.
```

## Orientações gerais para a aplicação da sequência didática 

- Antes de iniciar as atividades, é primordial que o professor realize uma leitura integral deste guia, identificando objetivos propostos em cada módulo e quais conhecimentos matemáticos serão mobilizados ao longo da sequência. 
- Apesar dos módulos estarem organizados em ordem crescente diante a sua complexidade, a duração de cada etapa deve ser adapta conforme a realidade da turma e disponibilidade de carga horária. 
- Quando possível, incentive a participação dos estudantes por meio da discussão, levantamento de hipóteses e socialização, em grupo, dos resultados obtidos no decorrer das atividades investigativas. 
- É necessário destacar, que este guia não tem o objetivo de proibir ou moralizar comportamentos relacionados às apostas, mas sim proporcionar aos estudantes capacidade para analisar de forma crítica essas situações por meio de argumentos fundamentados na Matemática. 
- Recursos necessários: 
    * Computador, dispositivos eletrônicos (Smartphone e Tablets); 
    * Laboratório de Informática, Acesso à internet (opcional); 
    * Excel ou Google Sheets; 
    * Projetor; 
    * Calculadora; 
    * Cartolina, Papel Madeira, Papel Duplex, e etc. 
    * Material gráfico para o infográfico. 

## Respostas esperadas das atividades 

### Módulo 1 

O estudante deverá identificar fatores como publicidade, influência das redes sociais, vulnerabilidade econômica, desejos imediatos de consumo e facilidades no acesso às plataformas. 

```{attention} Atenção
Professor, é importante aceitar outras respostas desde que tenham relação entre o contexto social e a tomada de decisão financeira.
```

### Módulo 2 

Reconhecer elementos de gamificação. 

```{attention} Atenção
Professor, é importante valorizar os exemplos dados pelos estudantes. 
```

### Módulo 3 

Espera-se que compreendam que Esperança Matemática negativa implica em perdas médias ao longo do tempo. 

```{attention} Atenção
Professor, alguns estudantes poderão realizar apenas uma jogada, pode ser necessário retomar o significado de valor esperado em muitas repetições. 
```

## Notas pedagógicas 

No Módulo 3, os estudantes tendem a acreditar que numa sequência com derrotas isso implicaria que as chances de vitória na jogada seguinte aumentam. Retome, se necessário, o conceito de independência dos eventos, com um exemplo diferente do exposto no guia, por exemplo: sorteio com reposição. 

No Módulo 4, os estudantes tendem a subestimar o efeito do tempo sobre os juros compostos. Explore os gráficos antes de apresentar as fórmulas. 

No Módulo 5, é interessante não transformar a atividade em um debate com base em opiniões. É importante pedir que os estudantes realizem as modelagens estudadas, para que consigam retomar com provas que evidenciem de fato suas opiniões. 

### Ampliações

Caso haja tempo disponível é interessante propor aos estudantes que alterem, por exemplo: 

- Taxa de juros; 
- Valor do aporte mensal; 
- Prazo; 
- Expectativa de ganho nas apostas; e etc. 

Posteriormente, eles podem fazer comparações entre os resultados diante essas mudanças. 

### Interdisciplinaridade 

- Matemática: 
    * Probabilidade, Função Exponencial, PG e Juros Compostos. 
- Língua Portuguesa: 
    * Leitura crítica das propagandas. 
- Sociologia: 
    * Consumo e Influência Digital. 
- Tecnologia 
    * Planilhas do Excel e Google Sheets. 

## Materiais complementares 

### Planilhas

- [Planilha do Módulo 3](m3-planilha.xlsx)
- [Planilha do Módulo 4](m4-planilha.xlsx)
- [Planilha do Módulo 5](m5-planilha.xlsx)

### Fórmulas Prontas 

- Microsoft Excel e Google Sheets 
    * Modelo das apostas: 
        - Resultado  
            * (Coluna `B`, Célula `B2`): `=SE(ALEATÓRIO()<=0,45; 1; -1)`
        - Saldo Acumulado 
            * (Coluna `C`, Célula `C2`): `=B2`
            * (Coluna `C`, Célula `C3`): `=C2+B3`

    * Modelo de aportes financeiros: 
        - Acumulado (sem rendimento): 
            * (Coluna `B`, Célula `B2`): `=50*A2`
        - Acumulado (juros compostos): 
            * (Coluna `C`, Célula `C2`): `=VF(0,8%; A2; -50; 0; 0)`

```{attention} Aviso
Professor, se o Google Sheets que o aluno abrir se tratar da versão em inglês, considere usar para a fórmula do valor futuro = future value, ou seja, `=FV(0.8%, A2, -50, 0, 0)`
```

## Considerações ao Professor 

Esta sequência didática foi idealizada para que os estudantes investiguem, por meio da Matemática, diferentes meios de destinação de seus recursos financeiros. Além de apenas ensinar conteúdos como Probabilidade, Esperança Matemática, Progressão Geométrica e Juros Compostos, procura-se desenvolver a capacidade de interpretação crítica de situações cotidianas, fundamentando as decisões financeiras com argumentos quantitativos.  

No decorrer da aplicação, valorize as hipóteses levantadas por seus alunos, incentive a discussão em grupo dos resultados e utilize os modelos matemáticos construídos como ferramentas de promoção à reflexão, não apenas a simples atividades de cálculo. O papel do professor é mediar o processo investigativo, conduzir os estudantes para que percebam que a Matemática contribui para escolhas financeiras mais conscientes e responsáveis. 