# Capítulo 1 -  Modelo de Dados do Python

## 10/08/2023

Meu Colab: https://colab.research.google.com/drive/1J0MlTbDPR-mJadULuILs1GeTQKtWQZk8#scrollTo=a9zoA7chuniy

O livro começa com um exemplo pouco convencional para quem viveu uma vida de frameworks web como eu.

O ponto inicial é: Como dar poder para uma classe padrão se beneficiar de métodos nativos como se fosse uma coleção?

Interessante pensar assim, no exemplo a gente consegue fazer um len() e acessar um indice direto da instância da classe, tudo isso só por escrever os métodos especiais len e getitem. A classe passa a ser iterável como um array, e não se trata de ter um atributo como array e usar ele, a classe em sí mesmo passa a ter este super-poder. Isso é realmente bem legal.

Eu fiz minha própria implementação para praticar, demorei um pouco para entender o sorted mas consegui fazer com lambda. É simples e bonito mesmo.

Até então, o que está pegando mesmo é a questão de dar super-poder para uma classe e reaproveitar os métodos padrões da linguagem para algum recurso customizado. E estou curtindo compreender que os métodos globais len, iter, str, etc na verdade executam os dunders especiais que eu criar nas minhas classes. Fica a advertcencia para não invocar métodos especiais diretamente e sim usar os globais.

Próxima Página 34 - Emulando tipos númericos

## 15/08/2023

Estou achando sensacional tudo isso do inicio da metaprogramação e a flexibilidade disponível para customizar classes.

Entendi que o objetivo disso tudo é dar ao usuário poder para que ele possa ter seus próprios recursos tão poderosos quanto os tipos nativos da linguagem.

O caso do len() não ser .len() faz todo sentido em termos de utilização agora, pelo que entendi, isso é assim pois o python calcula o tamanho dos tipos nativos de uma maneira própria, porém, se você precisar calcular tamanho de objetos próprios, poderá fazer do mesmo jeito, mantendo um padrão fácil de ler e simples de replicar.
O python faz a leitura do tamanho dos tipo nativos apenas lendo um atributo interno gravado pelo CPython.

Pelo que entendo de interpretador (nada kkk), quando a gente cria algo na linguagem primária (no caso python), esse algo provavelmente será criado em memória pela linguagem do interpretador. Inclusive, eu não faço a mínima ideia se o interpretador python é escrito em C,C++,sei lá.
Chuto que seja em C++.

O estudo de hoje reforçou sobre os métodos especiais e realmente isso tem aberto muito minha mente, parece que eu vivo na superfício das linguagens e há muito mais por vir. E olha que eu já vivi diversos cenários diferentes, com linguagens e contextos diferentes. Estou curtindo muito.

Isso finaliza o capítulo 1, foi bem enxuto e rápido, porém bastante interessante e estou ansioso pelo que ainda está por vir.

Próxima página 43 - Parte II - Estrutura de Dados