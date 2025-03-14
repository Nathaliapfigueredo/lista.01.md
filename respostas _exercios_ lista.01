
# Questões objetivas
**1) Considerando a execução do código abaixo, indique a alternativa correta e justifique sua resposta.**
```javascript
console.log(x);
var x = 5;
console.log(y);
let y = 10;
```
a) A saída será undefined seguido de erro **[CORRETA]**

b) A saída será 5 seguido de 10

c) A saída será undefined seguido de undefined

d) A saída será erro em ambas as linhas que utilizam console.log



**Justificativa**: Var x foi declarado no início do escopo, mas não inicializado, seu valor padrão é undefined até a linha onde "x = 5" é executada. Se tivesse sido inicializada com let teria dado erro e ficaria no Temporal Dead Zone, como acontece com o let y.



**2) O seguinte código JavaScript tem um erro que impede sua execução correta. Analise e indique a opção que melhor corrige o problema. Justifique sua resposta.**

```javascript
function soma(a, b) {
    if (a || b === 0) {
        return "Erro: número inválido";
    }
    return a + b;
}
console.log(soma(2, 0));
```

a) Substituir if (a || b === 0) por if (a === 0 || b === 0)  **[CORRETO]**

b) Substituir if (a || b === 0) por if (a === 0 && b === 0)

c) Substituir if (a || b === 0) por if (a && b === 0)

d) Remover completamente a verificação if (a || b === 0)


**Justificativa:** O código não está verificando corretamente se a ou b são iguais a zero. Para isso, cada uma das variáveis precisa ser igualada a zero, como “a === 0 || b === 0”.


______
**3) Ao executar esse código, qual será a saída no console? Indique a alternativa correta e justifique sua resposta.**
```javascript
function calcularPreco(tipo) {
    let preco;

    switch(tipo) {
        case "eletrônico":
            preco = 1000;
        case "vestuário":
            preco = 200;
            break;
        case "alimento":
            preco = 50;
            break;
        default:
            preco = 0;
    }

    return preco;
}

console.log(calcularPreco("eletrônico"));
```

a) O código imprime 1000.

b) O código imprime 200.  **[CORRETO]**

c) O código imprime 50.

d) O código gera um erro.



**Justificativa:** Um código com switch deve ser estruturado com cases e dentro de cada um uma ação seguida de break, o que não acontece no primeiro break desse switch. Dessa forma, mesmo que o console peça para imprimir o preco do case “eletrônico”, o código vai seguir rodando, assim passando para o case “vestuário”, preco 200 e finalizando com o break.

______
**4) Ao executar esse código, qual será a saída no console? Indique a alternativa correta e justifique sua resposta.**
```javascript
let numeros = [1, 2, 3, 4, 5];

let resultado = numeros.map(x => x * 2).filter(x => x > 5).reduce((a, b) => a + b, 0);

console.log(resultado);
```
a) 0

b) 6

c) 18

d) 24 **[CORRETO]**

**Justificativa:** isso acontece porque “.map(x => x * 2)” pega todos os elementos do array número e multiplica cada um por 2, o “.filter(x => x > 5)” filtra apenas os números maiores que 5 e o “.reduce((a, b) => a + b, 0)” soma os números resultantes partindo do valor inicial zero.


______
**5) Qual será o conteúdo do array lista após a execução do código? Indique a alternativa correta e justifique sua resposta.**

```javascript
let lista = ["banana", "maçã", "uva", "laranja"];
lista.splice(1, 2, "abacaxi", "manga");
console.log(lista);
```

a) ["banana", "maçã", "uva", "abacaxi", "manga", "laranja"]

b) ["banana", "abacaxi", "manga"]

c) ["banana", "abacaxi", "manga", "laranja"]   **[CORRETA]**

d) ["banana", "maçã", "uva", "abacaxi", "manga"]

Justificativa: o slice() é uma função que altera os elementos de uma lista, adicionando ou removendo. O 1 e 2 representam o índice dos elementos alterados e as strings "abacaxi" e "manga", os novos elementos adicionados. Assim substituindo maçã por abacaxi, e uva por manga.
______
**6) Abaixo há duas afirmações sobre herança em JavaScript. Indique a alternativa correta e justifique sua resposta**

I. A herança é utilizada para compartilhar métodos e propriedades entre classes em JavaScript, permitindo que uma classe herde os métodos de outra sem a necessidade de repetir código.  
II. Em JavaScript, a herança é implementada através da palavra-chave `extends`.


a) As duas afirmações são verdadeiras, e a segunda justifica a primeira.

b) As duas afirmações são verdadeiras, mas a segunda não justifica a primeira. **[CORRETA]**

c) A primeira afirmação é verdadeira, e a segunda é falsa.

d) A primeira afirmação é falsa, e a segunda é verdadeira.

**Justificativa:** A herança permite a reutilização do código sendo utilizada como no formado mencionado na afirmação I e o extends, de fato, é uma forma de implementar essa herança.No entanto,  a segunda afirmação não justifica a primeira pois existem outras formas de implementar essa herança além do extends.

______
**7) Dado o seguinte código. Indique a alternativa correta e justifique sua resposta.**

```javascript
class Pessoa {
  constructor(nome, idade) {
    this.nome = nome;
    this.idade = idade;
  }

  apresentar() {
    console.log(`Olá, meu nome é ${this.nome} e tenho ${this.idade} anos.`);
  }
}

class Funcionario extends Pessoa {
  constructor(nome, idade, salario) {
    super(nome, idade);
    this.salario = salario;
  }

  apresentar() {
    super.apresentar();
    console.log(`Meu salário é R$ ${this.salario}.`);
  }
}
```


I) A classe Funcionario herda de Pessoa e pode acessar os atributos nome e idade diretamente.  
II) O método `apresentar()` da classe Funcionario sobrepõe o método `apresentar()` da classe Pessoa, mas chama o método da classe pai usando `super`.  
III) O código não funciona corretamente, pois Funcionario não pode herdar de Pessoa como uma classe, já que o JavaScript não suporta herança de classes.

Quais das seguintes afirmações são verdadeiras sobre o código acima?

a) I e II são verdadeiras. **[CORRETO]**

b) I, II e III são verdadeiras.

c) Apenas II é verdadeira.

d) Apenas I é verdadeira.


**Justificativa:** A classe Funcionario estende (extends) a classe Pessoa, então herda seus atributos (nome e idade), assim esses atributos ficam acessíveis a Funcionário, confirmando a primeira afirmativa. Além disso, o método apresentar() de Funcionario sobrescreve o método apresentar() de Pessoa e ainda chama da classe pai o super.apresentar(), confirmando a afirmativa II.
A III está errada pois JavaScript suporta sim herança de classe utilizando extend.

______

**8) Analise as afirmações a seguir. Indique a alternativa correta e justifique sua resposta.**

**Asserção:** O conceito de polimorfismo em Programação Orientada a Objetos permite que objetos de diferentes tipos respondam à mesma mensagem de maneiras diferentes.  
**Razão:** Em JavaScript, o polimorfismo pode ser implementado utilizando o método de sobrecarga de métodos em uma classe.

a) A asserção é falsa e a razão é verdadeira.

b) A asserção é verdadeira e a razão é falsa. **[CORRETA]**

c) A asserção é verdadeira e a razão é verdadeira, mas a razão não explica a asserção.

d) A asserção é verdadeira e a razão é verdadeira, e a razão explica a asserção.


**Justificativa:** A segunda é falsa pois pois JavaScript não suporta métodos com o mesmo nome mais de uma vez dentro de uma classe.
______

# Questões dissertativas
9) O seguinte código deve retornar a soma do dobro dos números de um array, mas contém erros. Identifique os problema e corrija o código para que funcione corretamente. Adicione comentários ao código explicado sua solução para cada problema.

```javascript
function somaArray(numeros) {

    for (i = 0; i < numeros.size; i++) {
        soma = 2*numeros[i];
    }
    return soma;
}
console.log(somaArray([1, 2, 3, 4]));
```

CÓDIGO CORRIGIDO: 

```javascript 
soma=0; //no código anterior faltava a declaração da variável soma


function somaArray(numeros) {
   
    for (i = 0; i < numeros.length; i++) {  //aqui estava sendo utilizado numero.size propriedade que não existe no JavaScript, o correto é numeros.length
        soma += 2*numeros[i]; // aqui os valores multiplicados por dois não estavam sendo somados a variável soma
    }
    return soma;
}
console.log(somaArray([1, 2, 3, 4]));
```


______
10) Crie um exemplo prático no qual você tenha duas classes:

- Uma classe `Produto` com atributos `nome` e `preco`, e um método `calcularDesconto()` que aplica um desconto fixo de 10% no preço do produto.
- Uma classe `Livro` que herda de `Produto` e modifica o método `calcularDesconto()`, aplicando um desconto de 20% no preço dos livros.

Explique como funciona a herança nesse contexto e como você implementaria a modificação do método na classe `Livro`.

```javascript 
//cria a classe Produto
class Produto {
    // construtor da classe Produto que recebe os parâmetros nome e preco
    constructor(nome, preco) {
      this.nome = nome;
      this.preco = preco;
    }
 
    // método que calcula o desconto de 10% no preço do produto
    calcularDesconto() {
        return this.preco * 0.90;
    }
  }
 
  // cria a classe Livro que herda de Produto
  class Livro extends Produto {
    constructor(nome, preco, autor) {
      // chama o construtor da classe Produto
      super(nome, preco);
      this.autor = autor;
    }
 
    calcularDesconto() {
        return this.preco * 0.80; // Aplica 20% de desconto
    }
  }
 
// cria uma instância da classe Produto
let produto1 = new Produto("Camiseta", 100);
console.log(`${produto1.nome} com desconto: R$ ${produto1.calcularDesconto()}`);


let livro1 = new Livro("A teoria de tudo", 50, "Stephen Hawking");
console.log(`${livro1.nome}, do autor ${livro1.autor}, com desconto: R$ ${livro1.calcularDesconto()}`);
```

**Justificativa:** Primeiro, foi criada uma classe Produto, que possui um construtor que recebe os parâmetros nome e preco, e um método calcularDesconto que retorna o preço do produto com um desconto de 10%. Em seguida, foi criada a classe Livro, que herda de Produto. O construtor da classe Livro chama o construtor da classe Produto utilizando super(), garantindo que os parâmetros nome e preco sejam passados para essa classe. Além desses parâmetros, a classe Livro também recebe o atributo autor, que é exclusivo dessa classe. O método calcularDesconto foi reescrito na classe Livro para aplicar um desconto de 20% no preço do livro, modificando o return para refletir esse novo valor.

