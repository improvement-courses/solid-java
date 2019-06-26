# Solid
Curso de SOLID

### SRP (Single Responsibility Principle)
É um dos princípios SOLID, que o nome já diz, a ideia é ter uma única responsabilidade por classe. Ou seja, coesão.

### OCP
O OCP diz para escrevermos classes que sejam facilmente extensíveis (ou seja, abertas pra extensão). Dessa forma, mudar o comportamento da classe atual é fácil: basta passar outras implementações concretas das abstrações que ela depende.

Classes abertas para extensão, mas fechadas para modificação, também são mais coesas.

### DIP
O DIP nos diz para sempre dependermos de módulos que sejam mais estáveis que o módulo corrente. Abstrações devem depender de abstrações, e implementação deve depender de abstração.

Com isso, diminuímos o risco do acoplamento, afinal abstrações são estáveis, e tendem a não mudar frequentemente, diminuindo a propagação de problemas.

### Encapsulamento
Encapsular é esconder os detalhes da implementação dentro da classe. Dessa forma, as classes que farão uso dela, não saberão como ela funciona internamente. A vantagem disso é que conseguimos depois facilmente alterar a implementação, sem que ela impacte nas classes dependentes.

### Lei de Demeter
A Lei de Demeter, de maneira simples, diz para que você evite ao máximo fazer expressões como a.getB().getC().getD().acao(). O problema dessa cadeia, é que a classe que contém essa expressão, conhece muito sobre o comportamento da classe A, depois da classe B, até D. Se alguma delas mudar, a mudança será propagada para muitos lugares.

Diminuir a quantidade de invocações como essas ajuda você a encapsular melhor o comportamento e o funcionamento interno das classes.

