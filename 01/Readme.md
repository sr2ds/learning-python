# Modelo de Dados do Python

Meu Colab: https://colab.research.google.com/drive/1J0MlTbDPR-mJadULuILs1GeTQKtWQZk8#scrollTo=a9zoA7chuniy

O livro começa com um exemplo pouco convencional para quem viveu uma vida de frameworks web como eu.

O ponto inicial é: Como dar poder para uma classe padrão se beneficiar de métodos nativos como se fosse uma coleção?

Interessante pensar assim, no exemplo a gente consegue fazer um len() e acessar um indice direto da instância da classe, tudo isso só por escrever os métodos especiais len e getitem. A classe passa a ser iterável como um array, e não se trata de ter um atributo como array e usar ele, a classe em sí mesmo passa a ter este super-poder. Isso é realmente bem legal.

Eu fiz minha própria implementação para praticar, demorei um pouco para entender o sorted mas consegui fazer com lambda. É simples e bonito mesmo.

Até então, o que está pegando mesmo é a questão de dar super-poder para uma classe e reaproveitar os métodos padrões da linguagem para algum recurso customizado. E estou curtindo compreender que os métodos globais len, iter, str, etc na verdade executam os dunders especiais que eu criar nas minhas classes. Fica a advertcencia para não invocar métodos especiais diretamente e sim usar os globais.

Próxima Página 34 - Emulando tipos númericos