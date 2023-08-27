---
layout: post
title:  "Programação Orientada a Objetos para completos iniciantes"
date:   2023-08-27 20:20:00 +0100
categories: programação
author: Jader de Carvalho
thumbnail: https://arquivo.devmedia.com.br/marketing/img/programe-orientado-a-objetos.png
---

# Programação Orientada a Objetos para completos iniciantes

O intuito desse post é fazer uma introdução sobre a Programação Orientada a Objetos, também conhecida como POO (ou OOP que é a sigla em inglês para Object Oriented Programing) em seus aspectos mais básicos e teóricos para quem não faz a menor ideia do que isso signifique. Obviamente, haverá algum nível de aprofundamento teórico sobre o assunto, porém nada mirabolante. Portanto, se você é um programador iniciante ou não é nem iniciante ainda e apenas está curioso sobre o tema, esse post é para você.

## Por que Programação Orientada a Objetos?

Como se pode imaginar desde já, para falar desse assunto temos que dar uma pausa para pensar um pouco sobre o mundo real, sobre os objetos. Os objetos estão em todos os momentos das nossas vidas desde que nascemos, e é tão natural esse conceito que nem pensamos conscientemente que nossas roupas, nossos carros, nossos computadores e nossos óculos são objetos e tem algumas coisas em comum, por mais que não pareça. Todos os objetos tem CARACTERÍSTICAS e FUNÇÕES. Algumas das possíveis características de um carro são o fato de ter quatro rodas e volante e tem a função de nos transportar do ponto A ao ponto B assim como algumas das possíveis características de um par de óculos são o fato de terem uma estrutura e duas lentes e sua função é nos fazer enxergar melhor.

Dito isso, a Programação Orientada a Objetos é uma forma de entender e estruturar o nosso código de acordo com como são os objetos na vida real. A ideia é que a respeito do nosso código, tudo ou quase tudo sejam objetos interagindo com outros objetos, assim como um par de óculos (um objeto) repousa em cima de uma mesa (outro objeto).

A POO é uma forma de se estruturar um software que surgiu como uma alternativa a Programação Estruturada, que resumidamente é a arte de escrever um software de forma estruturada, com uma instrução após a outra, assim como funciona uma receita de bolo onde se tem uma lista de ingredientes e ações que são tomadas em uma ordem específica. Porém não é a intenção desse post nos aprofundarmos nessas diferenças, então voltemos à POO.

## Ok, mas como exatamente isso funciona?

Bom, a Programação Orientada a Objetos começa a ser implementada primeiro de forma abstrata, pensando-se em quais seriam os objetos do nosso software e como eles se relacionam e apenas depois ocorre a implementação de fato. Porém, temos que pensar um pouco mais antes disso. Na POO temos 3 conceitos básicos que precisam ser entendidos antes de pensarmos numa possível implementação de um software fictício. Esses conceitos básicos são três: CLASSES; ATRIBUTOS e MÉTODOS;

Uma Classe, assim como no mundo real, é a forma como tentamos classificar os objetos que tem características semelhantes. Por exemplo a classe dos animais vertebrados possui diversos animais que tem muitas características diferentes entre si, porém tem características em comum que fazem eles pertenceram a essa classe. Quando falamos das características em comum entre os animais da classe dos vertebrados podemos fazer um paralelo entre os Atributos em POO. As classes têm atributos, que são características que fazem diferentes objetos pertencerem a essa classe ou serem desse tipo. Já os Métodos são exatamente as funções que um objeto tem, sendo assim, nossas classes também tem métodos e se chama dessa forma por que são literalmente formas de se fazer uma ação.

Com certeza se você não está familiarizado com a Programação Orientada a Objetos esse último parágrafo ficou um pouco confuso, afinal de contas, o que tudo isso tem a ver com o mais importante na POO, ou seja, os objetos? E essa resposta é mais simples do que parece. Em Programação Orientada a Objetos uma Classe, na verdade, é apenas a receita de um objeto, é apenas o tipo do objeto. Ou seja, para criarmos um objeto quando estamos programando orientado a objetos, precisamos que esse objeto seja criado a partir de um tipo e esse tipo é uma classe que nós também definimos anteriormente.

Vamos pensar num exemplo para ficar mais fácil o entendimento. Imagine que precisamos criar um sistema para cadastrar os aniversários dos nossos amigos. Podemos assim começar a pensar em todas as coisas que poderiam ser objetos e em como esses objetos se relacionam. Uma coisa importante de se notar é que em POO utilizamos muito do artifício da abstração, logo, algo que na vida real nós não consideraríamos um objeto, aqui podemos considerar sem problemas. Por exemplo, queremos guardar informações a respeito dos nossos amigos, que são pessoas e nós sabemos que nesse contexto todas as pessoas tem algumas características em comum como nome e data de nascimento. Nesse exemplo seria bastante apropriado definirmos uma classe Pessoa com dois atributos: Nome e Data de Nascimento.

Devemos nos lembrar que criamos uma classe não um objeto ainda. Agora utilizando a linguagem de programação de nossas escolha, poderíamos partir para a criação de um objeto utilizando a classe Pessoa como modelo e definindo valores para os atributos nome e data de nascimento para esse objeto. Por exemplo um objeto chamado pessoa1 cujo valor do atributo nome seria Gabriel e o valor do atributo Data de Nascimento seria 29/12/1990. Agora poderíamos guardar os dados dessa pessoa (ou seja, dados que foram atribuídos aos atributos de um objeto) e assim teríamos um sistema simples para guardar o nome e aniversário dos nossos amigos.

## Muito interessante, mas por que só tem um objeto nesse exemplo?

Até aqui a ideia era apenas explicar os conceitos mais básicos de Programação Orientada a Objetos, porém, vamos evoluir nosso exemplo para nos aprofundarmos um pouco mais nesses e em outros conceitos.

A estrutura mais básica do nosso sistema já foi imaginada, porém esse sistema é muito simples. Além disso, muito pouco sobre POO foi utilizado então agora pensaremos em algo a mais para nosso exemplo. Vamos imaginar que além de guardar os aniversários dos nossos amigos queremos gravar também o telefone e o e-mail de cada um dos nossos amigos, como isso poderia ser feito?

A primeira ideia que nos vem à cabeça é: criarmos um atributo e-mail e um atributo telefone na classe Pessoa e dessa forma teremos tudo que precisamos para guardarmos os contatos dos nossos amigos assim que criarmos um objeto do tipo Pessoa, certo? Sim, isso definitivamente funcionaria, mas também não seria uma boa ideia. A ideia por de trás da Orientação a Objetos é pensarmos em maneiras de dividirmos tudo em objetos diferentes conversando entre si para abstrair e especializar cada pedaço do nosso código ao invés de fazermos tudo junto em um lugar só.

Uma pessoa, com certeza tem um nome e com certeza, nasceu em um dia específico, mas não necessariamente tem telefone ou e-mail. Número de telefone ou e-mail não se parecem com características de uma pessoa, se parecem mais com características de um Contato. Um contato não é um objeto palpável na vida real, porém aqui podemos nos valer da abstração para pensar em tudo como se fossem objetos, mesmo que não possam ser um objeto no mundo real. Então vamos imaginar que além de uma classe chamada Pessoa com atributos Nome e Data de Nascimento, agora criamos também no nosso sistema uma classe chamada Contato com atributos Telefone e E-mail.

Porém nossa abstração ainda não está completa. Se pensarmos um pouquinho perceberemos que um contato só existe referente a uma pessoa, porém nada nas nossas classes parecem dizer ainda que o contato X é referente a pessoa Y, e a solução para isso é simples (pelo menos nesse exemplo simples rs). Podemos criar dentro da classe contato, mais um atributo do tipo Pessoa.

Em Programação Orientada a Objetos, quando criamos uma classe estamos criando um tipo de dados. Sendo assim ao criarmos um atributo e-mail na classe contato, esse atributo seria provavelmente do tipo texto (não falarei dos tipos de dados específicos das linguagens de programação aqui), então poderíamos também criar uma classe do tipo Pessoa dentro da classe Contato para salvarmos então um contato que tenha um telefone, um e-mail, e uma pessoa a quem esses tipos de contatos pertencem.

Nós também poderíamos fazer o inverso e criar um atributo do tipo Contato na classe Pessoa, porém, logicamente falando não seria o mais adequado. Uma pessoa Pode ter um contato ou não, mas todo contato SEMPRE será referente a uma pessoa. Pode existir uma necessidade em outro sistema que faça com que faça mais sentido fazer dessa forma, porém pro nosso exemplo não é interessante.

Com isso, poderíamos agora criar um objeto chamado contato1 e atribuir os valores dos atributos e-mail como gabriel@email.com, telefone para 933 772 814 e o atributo pessoa como pessoa1, que é o objeto do tipo pessoa criado anteriormente com os atributos de nome Gabriel e data de nascimento 29/12/1990. E assim salvamos o contato do Gabriel assim como seu aniversário.