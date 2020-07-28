# Princípios de liderança

Esse markdown foi desenhado como um compilado do meu processo de desenvolvimento de liderança. Diferente de um artigo, ele é um documento evolutivo e iterativo. O objetivo é compartilhar os princípios e ferramentas principais em uma liderança técnica que possam ajudar a mais pessoas terem a experiência de liderança.

Agradeço a ideia vinda do [Kamil Sindi](https://github.com/ksindi/managers-playbook) e incrementada como todo apoio e Material da [a.karta](https://akarta.com.br/) e outras referências que serão mantidas como link.

# Sumário
- [Princípios de liderança](#princ-pios-de-lideran-a)
- [Sumário](#sum-rio)
- [Introdução](#introdu--o)
- [Time](#time)
- [O papel e características do líder neste time](#o-papel-e-caracter-sticas-do-l-der-neste-time)
- [Lean Management](#lean-management)
  * [Princípio do baixo acoplamento](#princ-pio-do-baixo-acoplamento)
  * [Principio da alta iteração](#principio-da-alta-itera--o)
  * [Princípio das pequenas entregas](#princ-pio-das-pequenas-entregas)
  * [Princípio da automação](#princ-pio-da-automa--o)
  * [Princípio da visibilidade](#princ-pio-da-visibilidade)
  * [Princípio da diversidade](#princ-pio-da-diversidade)
- [Cerimônias e reuniões](#cerim-nias-e-reuni-es)
  * [Daily](#daily)
  * [Retrospectiva](#retrospectiva)
  * [Planning](#planning)
  * [One on Ones](#one-on-ones)
    + [1:1s de futuro profissional](#1-1s-de-futuro-profissional)
    + [1:1s de time](#1-1s-de-time)
    + [1:1s de projeto](#1-1s-de-projeto)
    + [1:1s sobre feedback sobre o trabalho como lider](#1-1s-sobre-feedback-sobre-o-trabalho-como-lider)
    + [Primeiras 1:1s com meus líderes](#primeiras-1-1s-com-meus-l-deres)
  * [Alinhamento de Objetivos (Goal Setting e Tour of Duty)](#alinhamento-de-objetivos--goal-setting-e-tour-of-duty-)
  * [Comemorações e Entrega](#comemora--es-e-entrega)
- [Processos e ferramentas](#processos-e-ferramentas)
- [Motivação do time](#motiva--o-do-time)
- [Organização Pessoal](#organiza--o-pessoal)
- [Links e Livros](#links-e-livros)

<!-- <small><i><a href='http://ecotrust-canada.github.io/markdown-toc/'>Table of contents generated with markdown-toc</a></i></small> -->


# Introdução

> Kintsugi ("emenda de ouro") é uma antiga arte japonesa que consiste em reparar cerâmica quebrada com pó de ouro ou algum material com brilho, tornando-a uma peça única pois suas rachadoras beiram o impossível de se reproduzir. Como resultado, a peça restaurada se torna muito mais valiosa.

Como metáfora (e até filosofia!), cada pessoa traz consigo uma história e diversas "rachaduras" que as fazem únicas. As história e as imperfeições de cada pessoa são especiais e devem ser respeitadas como tal. O líder, neste cenário, é alguém com um papel tático dentro de uma organização capaz de perceber as competências (peças) que o time possui, uní-las em cima de algo valioso como um objetivo.

# Time

> “In teams which scored highly on architectural capabilities, little communication is required between delivery teams to get their work done.[...] In other words, architecture and teams are loosely coupled. To enable this, we must also ensure delivery teams are cross-functional, with all the skills necessary to design, develop, test, deploy, and operate the system on the same team.”

*Jez Humble; Nicole Forsgren; Gene Kim - Accelerate*

Um time é uma célula auto-suficiente, geralmente cross-functional e com o mínimo de interfaces composta por diversos papéis e que respeite a regra do [Two Pizzas Team](https://buffer.com/resources/small-teams-why-startups-often-win-against-google-and-facebook-the-science-behind-why-smaller-teams-get-more-done/) (o tamanho do time no deve superar o que duas pizzas são capazes de alimentar em uma noite escura de inverno) onde todos são responsáveis pelo resultado do produto/projeto.

# O papel e características do líder neste time

Disclaimer: Os pontos abaixos são competências propostas pelos materias e experiências. No entanto, encontrar alguém capaz de ser tudo isso sempre é meio unicórnio

No cenário de Desenvolvimento de Software, o líder é aquele que tem a responsabilidade de:
* Escutar, entender e cuidar da individualidade de cada pessoa
* Encontrar aprendizado das falhas ao invés de culpados [1] 
* Comunicar um forte senso de propósito [1] e elevar a barra do time
* Investir no desenvolvimento do liderado, inclusive dando tempo, espaço e recurso para experimentar e aprender [1] 
* Ser um facilitador, um meio de campo, entre as diferentes forças que interagem em um time
* Evitar: Ser gargalo, a palavra final em decisões técnicas, participar somente em cerimônias e, principalmente, não ter filtro emocional

E para isso ele pode ter algumas características como:
* Visão[1]: Entendimento claro onde estamos e onde devemos estar em um futuro factível (2 anos? 5? Vai do contexto) 
* Comunicação inspiracional[1]: Comunica inspirando e motivando, mesmo em cenários incertos.
* Desafiar intelectualmente[1]: Incentiva ao time pensar sobre o problema de formas diferentes.
* Supportive leadership[1]: Demonstra cuidado e consideração pelas pessoas e seus sentimentos
* Reconhecimento pessoal[1]: Reconhece o cumprimento de metas e melhorias na qualidade do trabalho; elogia pessoalmente.

O lider geralmente é a figura que representa a empresa para aquele time. Sendo assim, é perceptível que as pessoas gostam de ver a conexão do seu trabalho em impactos positivos para os clientes e, consequentemente, alinhando-se ao propósito da empresa. Isso torna possível uma melhoria na qualidade da entrega do Software e Performance organizacional.

[1] *Retirados de Jez Humble; Nicole Forsgren; Gene Kim - Accelerate*

# Lean Management

## Princípio do baixo acoplamento

> In teams which scored highly on architectural capabilities, little communication is required between delivery teams to get their work done. [Also,] the architecture of the system is designed to enable teams to test, deploy, and change their systems without dependencies on other teams.
> [Because of that,] high-performing group [...] can do most of our testing without requiring an integrated environment. We can and do deploy or release our application independently of other applications/ services it depends on.

*Jez Humble; Nicole Forsgren; Gene Kim - Accelerate*

EXPLICAÇÃO

> The goal is for your architecture to support the ability of teams to get their work done— from design through to deployment— without requiring high-bandwidth communication between teams. [...] Use of bounded contexts and APIs as a way to decouple large domains into smaller, more loosely coupled units, and the use of test doubles and virtualization as a way to test services or components in isolation.

*Jez Humble; Nicole Forsgren; Gene Kim - Accelerate*

Para tudo isso acontecer, reforça o desafio de ter um time com diversas habilidades nele:

> Specialized roles create efficiencies within each segment while potentially creating inefficiencies across the entire life cycle.

*(Netflix Technology Blog - Full Cycle Developers at Netflix — Operate What You Build)[https://netflixtechblog.com/full-cycle-developers-at-netflix-a08c31f83249]*

> ensure delivery teams are cross-functional, with all the skills necessary to design, develop, test, deploy, and operate the system on the same team.

*Jez Humble; Nicole Forsgren; Gene Kim - Accelerate*

## Principio da alta iteração 

> [product] actively and regularly seek customer feedback and incorporate this feedback into the design of their products.
> development teams have the authority to create and change specifications as part of the development process without requiring approval.
> Working in small batches enables short lead times and faster feedback loops.
> One of the points of Agile development is to seek input from customers throughout the development process, including early stages.

> Our key hypothesis in asking these questions was that teams implementing continuous delivery practices and taking an experimental approach to product development will build better products, and will also feel more connected to the rest of their organization. This, in turn, creates a virtuous cycle: by creating higher levels of software delivery performance, we increase the rate at which teams can validate their ideas, creating higher levels of job satisfaction and organizational performance.

## Princípio das pequenas entregas

> Even though working in small chunks adds some overhead, it reaps enormous rewards by allowing us to avoid work that delivers zero or negative value for our organizations.
> We found that external approvals were negatively correlated with lead time, deployment frequency, and restore time, and had no correlation with change fail rate.
> High-performing teams were more likely to incorporate information security into the delivery process.
*Jez Humble; Nicole Forsgren; Gene Kim - Accelerate*

## Princípio da automação

> Automated unit and acceptance tests should be run against every commit to version control to give developers fast feedback on their changes. [...] Developers should be able to run all automated tests on their workstations
> No one should be saying they are “done” with any work until all relevant automated tests have been written and are passing.
> when teams practice CD, deployment to production is not an enormous, big-bang event— it’s something that can be done during normal business hours as a part of regular daily work.
> they help to decrease deployment pain and team burnout.
> improvements in CD brought payoffs in the way that work felt. This means that investments in technology are also investments in people, and these investments will make our technology process more sustainable
> changes should only be applied to production using a fully automated process that forms part of a deployment pipeline. That is, no changes should be able to be made to production unless they have been committed to version control, validated by the standard build and test process, and then deployed through an automated process triggered through a deployment pipeline.
*Jez Humble; Nicole Forsgren; Gene Kim - Accelerate*

Documentação faz parte de automação pois deixa o time livre para nao tirar duvidas

## Princípio da visibilidade 

> Last but not least, managers should make performance metrics visible and take pains to align these with organizational goals, and should delegate more authority to their employees.
*Jez Humble; Nicole Forsgren; Gene Kim - Accelerate*

## Princípio da diversidade

> Diversity matters. Research shows that teams with more diversity with regard to gender or underrepresented minorities are smarter (Rock and Grant 2016), achieve better team performance (Deloitte 2013), and achieve better business outcomes [...] It is also important to note that diversity is not enough. Teams and organizations must also be inclusive.
*Jez Humble; Nicole Forsgren; Gene Kim - Accelerate*

# WIP

<!--

# Cerimônias e reuniões

## Daily

**Objetivo:** 

**Premissa:** 

**Duração:** 

##  Retrospectiva

**Objetivo:** 

**Premissa:** 

**Duração:** 

##  Planning

**Objetivo:** 

**Premissa:** 

**Duração:** 

## One on Ones

**Objetivo:** Esta é a cerimônia mais importante na construção de um relacionamento líder-liderado. É aqui que acompanhamos:
- O passado: Feedback sobre comportamentos e entregas
- O presente: Performance, clima e relacionamento com a equipe
- O futuro: Tour of duty e alinhamento de expectativas

Este é o momento que deve ser individualizado: o que funciona para uma pessoa pode não funcionar para outra (ou até mesmo para a mesma pessoa em um tempo diferente)

**Premissa:** Ele tem como premissa as [4 fases do aprendizado](https://focuslife.com.br/4-fases-do-aprendizado-pnl/)

![Fases do Aprendizado](./images/fases-do-aprendizado.png)

**Duração:** Ela pode variar de pessoa para pessoa mas geralmente é uma reunião de 30 a 40 minutos. Onde segue-se geralmente esta estrutura:
1. Abrir espaço para deixar o liderado trazer o tópico principal (Começar sempre com: E aí, como está sendo a semana?)
2. Trazer um dos tópicos abaixo, se tiver tempo.
3. Finalizar a 1:1 com algo "O que podemos fazer para evoluirmos no que falamos hoje? Vamos chegar a uma solução em conjunto?"

### 1:1s de futuro profissional
* Como você vê o seu futuro profissional? O que você acredita que a empresa já conseguiu te ajudar neste sentido? Como a empresa consegue ajudar nas conquistas que você almeja? Como posso ajudar?
* Você sente que está progredindo nos seus grandes objetivos aqui?
* Seu trabalho é o que você esperava quando aceitou? Como você descreveria o ambiente de trabalho no time?

### 1:1s de time
* Hoje você tem um ponto focal no time? Alguém que você admira? Com quem você tem mais dificuldade em trabalhar? Por quê?
* Dos valores da empresa, você acredita que estamos falhando em algum?

### 1:1s de projeto
* Como esse projeto está indo? O que podemos fazer para fazermos melhor? Algo te travando? Algo não está claro? Posso ajudar em algo
* Dentro deste projeto, qual seria o resultado ideal? E como podemos alcançá-lo na sua opinião?

### 1:1s sobre feedback sobre o trabalho como lider
* Como lider, o que não estou fazendo para ajudar o seu dia-a-dia?
* Como lider, o que estou fazendo para ajudar o seu dia-a-dia?
* O que não deveria estar fazendo e estou?

### Primeiras 1:1s com meus líderes
Assim como os liderados, seus líderes precisam ter clareza sobre seu trabalho e você precisa ter clareza das expectativas deles

* O que você espera do time no final do quarter? Quais são os critérios de sucesso (padrão de desempenho, entregas, métricas, iniciativas) que devem avaliar minha performance?
* Qual é o seu maior medo sobre nossa temática?
* Quais desafios da área meu time é diretamente responsável?
* Como vemos minha contribuição para esse momento do time/área/negócio?

## Alinhamento de Objetivos (Goal Setting e Tour of Duty)

> "Uma vida com propósito é aquela em que eu entenda as razões pelas quais faço o que faço e pelas quais claramente deixo de fazer o que não faço." 

> "Até algum tempo atrás, a vida era muito menos complexa e a intenção principal era sobreviver. Isto é, obter recursos para montar uma família e ter um patrimônio que se pudesse deixar de herança. Como a sociedade hoje é mais focada no indivíduo, a ideia de propósito está marcada por um conceito que já existiu e voltou com força: o da realização."

*["Por que fazemos o que fazemos?" - Mario Sergio Cortella](https://www.amazon.com/Por-que-fazemos-Portuguese-ebook/dp/B01JT2I3DA/)*

Alinhar objetivos é essencial para uma boa comunicação líder-liderado. A importância de chegar a objetivos comuns do time e pessoais é que eles deixam clara a sua relação com as pessoas do time e como (Key Results) devem ser alcançados.

PESQUISAR UM POUCO MAIS SOBRE OKRs

Idealmente trabalha-se com 2 tipos de Goals para um determinado tempo (Semestre/Trimestre):
1. Objetivo de entrega ou do time: Como um time, precisamos estar alinhados com os objetivos da empresa. Neste sentido, os objetivos aqui explorados são alinhados para que consigamos atingir um marco dentro da Organizaço e conseguir novos investimentos. 
2. Objetivo pessoal ou de desenvolvimento: Toda pessoa que está no grupo tem o interesse de se desenvolver

Os objetivos de time alinham somente que iremos passar de um ponto A para um ponto B.

```
A----|-----|-----|----> B(performance)
```

Para uma organização continuar inovando. Esta passagem de fase muitas vezes não é suficiente. Fazer do mesmo jeito do que fazíamos ontem pode ser o primeiro passo para o fracasso. No entanto, alinhar as goals pessoais conseguem transformar a visão das pessoas, propondo e explorando novas soluções, transformando o tour de uma pessoa:

```

                    /--> C,D(desenvolvimento)     ^
                   /                              | proximos 
                  /                               |
A----|-----|-----|----> B(performance)            | tours
```

Para o desenvolvimento pessoal, existe um framework: 70/20/10 
* 70% do tempo na prática
* 20% do tempo com pessoas/mentores
* 10% do tempo em um estudo formal como livros ou cursos


PESQUISAR UM POUCO MAIS SOBRE TOUR OF DUTY

## Comemorações e Entrega

> "A coisa mais incrível de vencer não é a vitória em si. É poder contar, ensinar outras pessoas sobre como você fez, por que fez, de que maneira fez, com que considerações fez e o que levou em conta. São os valores que você pratica que contam."

*["Seja foda! - Caio Carneiro"](https://www.amazon.com.br/Seja-foda-Portuguese-Caio-Carneiro-ebook/dp/B079GZM3P5)*

# Motivação do time

> "Rotina não é monotonia, [...] a rotina consiste em uma série de procedimentos-padrão com os quais um processo completa. E esse nível de repetibilidade é o que torna a rotina mais adequada. [...] A monotonia é a morte da motivação. As pessoas [...] tentam alterar a situação quando veem o risco de monotonia”

*["Por que fazemos o que fazemos?" - Mario Sergio Cortella](https://www.amazon.com/Por-que-fazemos-Portuguese-ebook/dp/B01JT2I3DA/)*

> The most important characteristic of high-performing teams is that they are never satisfied: they always strive to get better.
*Jez Humble; Nicole Forsgren; Gene Kim - Accelerate*

Em rituais como 1:1 temos bastante uma visão da pessoa sobre suas motivações. No entanto, é importante enteder pessoas como um grupo.

ENTENDER QUE TODOS TEMOS INTERESSE DENTRO DO GRUPO

PODCAST DO NARUHODO

TEORIA DE GRUPO

Segurança Psicológica (fearless organization / Coragem Psicologica)- Fenômeno de Grupo. Oportunidade de enxergar no grupo que estou:
* Expressar
* Interagir
* Aprender
* Pertencer

"Nada melhor para desmotivar uma boa pessoa é tolerar uma ruim"

# Organização Pessoal

Uso de uma só agenda porque você é um só!

# Links e Livros

- Accelerate
- Meus artigos https://medium.com/@felipecdo/o-que-software-livre-ainda-tem-para-nos-ensinar-c0f3c5c330aa
-->
