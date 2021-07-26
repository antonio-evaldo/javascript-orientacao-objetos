# Curso de JavaScript Orientado a Objetos

## Módulo 1

Foi aprendido sobre:

* Criar Classes
* O que são atributos
* Instância/Objeto
* Operador `new`

## Módulo 2

Foi aprendido sobre:

* Criação de métodos
* Palavra chave `this`
* Encapsulamento
* Proposta de atributos privados

A [proposta](https://github.com/tc39/proposal-class-fields#private-fields) de se usar `#` para atributos privados já foi feita há anos e já está bem avançada, com o Node.js já a implementando, mas a linguagem em si ainda não a adotou. Ou seja, não deve ser utilizada em produção, e a convenção atualmente feita é para se utilizar `_`. Isso não torna os atributos e métodos privados de verdade, mas os desenvolvedores saberão que não podem ser modificados.

* `return` e *early return*

## Módulo 3

Foi aprendido sobre:

* Package.json
* Modules
* import/export

Os Modules do JS foram implementados no ES6, trazendo novas palavras-chave como `import` e `export`. Cada arquivo do JS pode ser tratado como um módulo e isso deve ser especificado no arquivo `package.json` com a configuração `"type": "module"`, caso contrário o Node indicará um erro. Além disso, alguns navegadores não suportam essa funcionalidade e não é recomendado utilizar os modules diretamente em produção, mas algumas bibliotecas e frameworks permitem que trabalhemos com eles sem problemas, pois transcompilam o código para que qualquer navegador consiga ler.

* Vantagens de se usar classes

O código tem potencial para se tornar bastante reaproveitável e legível, quando fazemos, por exemplo, integração entre diferentes instâncias de objetos. No caso dessa aula, foi feito o método `transferir`, onde usamos a própria instância da conta para fazer um saque e usamos a instância da outra conta que recebemos por parâmetro para fazer o depósito.

* Tipos de valor e tipos de referência
* Alterando dinamicamente um objeto

No JavaScript, tipos que não são primitivos guardam na variável um valor da referência para, por exemplo, o objeto. Por isso que quando passamos a instância de um objeto como parâmetro de uma métodos, podemos nos aproveitar de todas as informações da instância dentro da declaração do método, alterando dinamicamente a instância do objeto.
