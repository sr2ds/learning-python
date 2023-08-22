# Capítulo 2 - Uma coleção de sequências

Colab: https://colab.research.google.com/drive/1b9ORzk3p3ZnvnsiYrAhxdJ2N6nJMzql1?usp=sharing

## 22/08/2023

Bora iniciar hoje o capítulo 2!

Começamos com listcomps, eu já utilizei isso algumas vezes, achei irado mas não estudei e nem fui a fundo.
A ideia retornar dados de uma lista para outra com uma iteração simplificada, segundo o livro isso além de ser mais elegante (concordo) também é mais perfomático do que um for basico em alguns casos.

Dei uma brincada no colab e é muito legal mesmo esse lance, confere o link de cima!
Fica bem bonito o código usando listcomps e 'quase' simples como em JS:

```js
people = [{"name": 'David', "gender": "M"}, {"name": "Amanda", "gender": "F"}]
male = people.filter(p => p.gender == 'M')
```

```python
people = [{"name": 'David', "gender": "M"}, {"name": "Amanda", "gender": "F"}]
male = [p for p in people if p["gender"] == 'M']
```

Provalvemente dê pra fazer com filter lambda em python também, mas aí ficará menos legível ainda, eu acho.

Eu tenho bastante interesse em entender mais sobre geradores, por agora o livro já começou a falar mas bem superficial, será abordado mais no futuro.
Por agora, o que eu pude entender é que fazer um for em uma expressão geradora faz com que os dados gerados não sejam armazenados em memória, por são gerados em tempo de execução.
Em outras palavras, eu não entendi o suficiente kkkk
Mas neste ponto do livro ele apenas falou que isso existe e deu dois exemplos simples.
No colab eu refiz um bloco com genexpr pra testar a performance e PARECE mais rápido mesmo, questão de milésimos de segundos mas já parece mais rapido para coisas pequenas.
Ajustei os números do meu range para números maiores e nestes casos maiores, o genexpr não ganha do simples listcomps.. Mas claro, eu não sei testar o suficiente para analisar isso.

Próxima página: 52