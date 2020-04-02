# Manual do Iniciante em JavaScript


### JavaScript é uma das linguagens de programação mais populares do mundo.

Acredito que é uma ótima opção para sua primeira linguagem de programação.

Utilizamos JavaScript principalmente para criar

- Websites
- Aplicações Web
- Aplicações do lado do servidor usando Node.js

mas o JavaScript não limita-se a essas coisas e também pode ser usado para

- Criar Aplicações Mobile usando ferramentas como o React Native
- Criar programas para Microcontroladores e Internet das Coisas
- Criar aplicativos Smartwatch

Basicamente, pode fazer qualquer coisa. É tão popular que tudo de novo que aparece, em algum momento, terá um tipo de integração com o JavaScript. 

JavaScript é uma linguagem de programação que é:

- **alto nível**: fornece abstrações que permitem ignorar os detalhes da máquina em que está sendo executada. 
Ela gerencia a memória automaticamente com um coletor de lixo, então você pode se concentrar no código em vez de gerenciar a memória, como outras linguagens como C precisariam. Além disso, fornece muitas construções que permitem lidar com variáveis e objetos altamente poderosos.

- **dinâmica**: ao contrário das linguagens de programação estáticas, uma linguagem dinâmica executa em tempo de execução muitas das coisas que uma linguagem estática faz no tempo de compilação.
Isso tem prós e contras e fornece recursos poderosos como a digitação dinâmica, a ligação tardia, a reflexão, a programação funcional, a alteração do tempo de execução do objeto, fechamentos e muito mais. Não se preocupe se essas coisas lhe forem desconhecidas - você as conhecerá até o final do curso.

- **fortemante tipada**: uma variável não impõe um tipo. Você pode reatribuir qualquer tipo a uma variável, por exemplo, atribuindo um número inteiro a uma variável que contém uma sequência.

- **fracamente tipada**: em oposição à fortemente tipada, as linguagens vagamente (ou fracamente) tipadas não impõem o tipo de um objeto, permitindo  assim mais flexibilidade, mas nos negando a segurança e a verificação de tipo (algo que o TypeScript - que se baseia no JavaScript - fornece)

- **interpretada**: é comumente conhecida como linguagem interpretada, o que significa que ela não precisa de um estágio de compilação para que um programa possa ser executado, o que é necessário em C, Java e Go, por exemplo. Na prática, por motivos de desempenho, os navegadores compilam o JavaScript antes de executá-lo, mas isso é transparente para você - não há etapa adicional envolvida.

- **multi-paradigma**: a linguagem não impõe nenhum paradigma de programação específico, ao contrário do Java, por exemplo, que força o uso da programação orientada a objetos, ou do C que força a programação imperativa. É possível escrever JavaScript usando um paradigma orientado a objetos, usando protótipos e a nova sintaxe de classes (a partir do ES6). Você pode escrever JavaScript em um estilo de programação funcional, com suas funções de primeira classe, ou mesmo em um estilo imperativo (tipo C).

Caso você esteja se perguntando, o JavaScript não tem nada a ver com Java, é uma má escolha de nome, mas temos que viver com ele.

## Sumário 

1. [Um pouco de história]()
2. [Apenas JavaScript]()
3. [Uma breve introdução à sintaxe do JavaScript]()
4. [Ponto e vírgula]()
5. [Values]()
6. [Variáveis]()
7. [Tipos]()
8. [Expressões]()
9. [Operadores]()
10. [Regras de precedência]()
11. [Operadores de comparação]()
12. [Condicionais]()
13. [Arrays]()
14. [Strings]()
15. [Loops]()
16. [Funções]()
17. [Arrow Functions]()
18. [Objetos]()
19. [Propriedades do objeto]()
20. [Métodos de objeto]()
21. [Classes]()
22. [Herança]()
23. [Programação assíncrona e callbacks]()
24. [Promises]()
25. [Async and Await]()
26. [Variável Escopo]()
27. [Conclusão]()
--------

## Um pouco de história 

Criado em 1995, o JavaScript percorreu um longo caminho desde seu humilde começo .

Foi a primeira linguagem de script suportada nativamente pelos navegadores da Web e, graças a isso, ganhou uma vantagem competitiva sobre qualquer outra linguagem e hoje ainda é a única linguagem de script que podemos usar para criar aplicativos da Web.

Existem outras lingugens, mas todas devem ser compilados para JavaScript - ou mais recentemente para o WebAssembly, mas essa é outra história.

No começo, o JavaScript não era tão poderoso como é hoje, sendo usado principalmente para animações sofisticadas e para a maravilha conhecida na época como HTML Dinâmico.

Com as crescentes necessidades exigidas pela plataforma da Web (que continua a exigir), o JavaScript também teve a responsabilidade de crescer para acomodar as necessidades de um dos ecossistemas mais usados no mundo.

Agora o JavaScript também é amplamente usado fora do navegador. A ascensão do Node.js nos últimos anos desbloqueou o desenvolvimento de back-end, uma vez dominado por Java, Ruby, Python, PHP e linguagens mais tradicionais do lado do servidor.

Atualmente, o JavaScript também é uma linguagem que alimenta bancos de dados e muitos aplicativos. Além disseo, é possível desenvolver aplicativos incorporados, aplicativos móveis, aplicativos de TV e muito mais. O que começou como uma pequena linguagem dentro do navegador agora é a linguagem mais popular do mundo.


## Apenas JavaScript

Às vezes, é difícil separar o JavaScript dos recursos do ambiente em que é usado.

Por exemplo, a linha console.log () que você pode encontrar em muitos exemplos de código não é JavaScript. Em vez disso, faz parte da vasta biblioteca de APIs fornecidas no navegador.


Da mesma forma, no servidor às vezes pode ser difícil separar os recursos da linguagem JavaScript das APIs fornecidas pelo Node.js.

É um recurso específico fornecido pelo React ou pelo Vue? É "JavaScript simples" ou ,como costuma ser chamado, "Vanilla JavaScript"?

Neste livro, falo sobre JavaScript, a linguagem.

Sem complicar seu processo de aprendizado com coisas que estão fora dele e fornecidas por ecossistemas externos.

## Uma breve introdução à sintaxe do JavaScript

Nesta pequena introdução, quero falar sobre 5 conceitos:

- espaço em branco
- case sensitive
- literais
- identificadores
- comentários

#### Espaço em branco

JavaScript não considera espaço em branco significativo. Espaços e quebras de linha podem ser adicionados da maneira que você desejar, pelo menos em teoria.

Na prática, você provavelmente manterá um estilo bem definido e seguirá o que as pessoas costumam usar, e aplicará isso usando um linter ou uma ferramenta de estilo como o Prettier.

Por exemplo, eu sempre uso 2 caracteres de espaço para cada recuo.

#### Case sensitive 

JavaScript é case sensitive. Uma variável chamada **something** é diferente de **Something**.

O mesmo vale para qualquer identificador.

#### Literais

Definimos literal como um valor gravado no código-fonte, por exemplo, um número, uma sequência de caracteres, um booleano ou construções mais avançadas, como Object Literals ou Array Literals:

```
5
'Test'
true
['a', 'b']
{cor: 'vermelha', forma: 'Retângulo'}
```

#### Identificadores

Um identificador é uma sequência de caracteres que pode ser usada para identificar uma variável, uma função ou um objeto. Pode começar com uma letra, o cifrão $ ou um sublinhado _ e pode conter dígitos. Usando Unicode, uma letra pode ser qualquer caractere permitido, por exemplo, um emoji 😄.

```
Test
test
TEST
_test
Test1
$test
```

O cifrão é comumente usado para referenciar elementos DOM.

Alguns nomes são reservados para uso interno do JavaScript e não podemos usá-los como identificadores.

#### Comentários

Os comentários são uma das partes mais importantes de qualquer programa, em qualquer linguagem de programação. Eles são importantes porque nos permitem anotar o código e adicionar informações importantes que, de outra forma, não estariam disponíveis para outras pessoas (ou nós mesmos) lendo o código.

Em JavaScript, podemos escrever um comentário em uma única linha usando //. Tudo depois de // não é considerado como código pelo interpretador JavaScript.

Como isso:
```
// um comentário
true // outro comentário
```

Outro tipo de comentário é um comentário com várias linhas. Começa com / * e termina com * /.

Tudo no meio não é considerado como código:
```
/* algum tipo
de
comentário 

*/
```

# Ponto e vírgula

Cada linha em um programa JavaScript é opcionalmente encerrada usando ponto e vírgula.

Eu disse opcionalmente, porque o intérprete JavaScript é inteligente o suficiente para introduzir ponto e vírgula para você.

Na maioria dos casos, você pode omitir ponto-e-vírgula dos seus programas sem nem pensar nisso.

Este fato é muito controverso. Alguns desenvolvedores sempre usam ponto e vírgula, outros nunca usam ponto e vírgula e você sempre encontrará código que usa ponto e vírgula e código que não.

Minha preferência pessoal é evitar ponto e vírgula, então meus exemplos no livro não os incluem.

# Valores (values) 

Uma string <kbd>hello</kbd> é um valor.

Um número <kbd>12</kbd> é um valo.

<kbd>Hello</kbd> e <kbd>12</kbd> são valores. String e number são os tipos desses valores.

O tipo é o tipo de valor, sua categoria. Temos muitos tipos diferentes no JavaScript, e falaremos sobre eles em detalhes mais adiante. Cada tipo tem suas próprias características.

Quando precisamos fazer uma referência a um valor, atribuímos a uma variável.

A variável pode ter um nome e o valor é o que está armazenado em uma variável, para que possamos acessá-lo posteriormente através do nome da variável.

# Variáveis

Uma variável é um valor atribuído a um identificador, para que você possa fazer referência e usá-lo posteriormente no programa.

Isso ocorre porque o JavaScript é fracamente tipado, um conceito sobre o qual você ouvirá com frequência.

Uma variável deve ser declarada antes que você possa usá-la.

Temos duas maneiras principais de declarar variáveis. O primeiro é usar <kbd>const</kbd>:
```
const a = 0
```

A segunda é usar <kbd>let</kbd>:
```
let a = 0 
```

Qual é a diferença?

<kbd>const</kbd> define uma referência constante a um valor. Isso significa que a referência não pode ser alterada. Você não pode reatribuir um novo valor a ele.

Com a opção <kbd>let</kbd>, você pode atribuir um novo valor a ele.

Por exemplo, você não pode fazer isso:
```
const a = 0
a = 1
```
Porque você receberá um erro: <kbd>TypeError: Assignment to constant variable.</kbd>

Por outro lado, você pode fazer isso usando <kbd>let</kbd>:
```
let a = 0
a = 1
```

<kbd>const</kbd> não significa "constante" da maneira que outras línguas como C significam. Em particular, isso não significa que o valor não pode ser alterado - significa que não pode ser reatribuído. Se a variável apontar para um objeto ou um array (veremos mais sobre objetos e arrays posteriormente), o conteúdo do objeto ou da array poderá ser alterado livremente.

As variáveis <kbd>const</kbd> devem ser inicializadas no momento da declaração:

```
const a = 0
```

mas o valor de <kbd>let</kbd> pode ser inicializado depois:
```
let a 
let a = 0
```

Você pode declarar várias variáveis ao mesmo tempo na mesma instrução:
```
const a = 1, b = 2
let c = 1, d = 2
```

Mas você não pode redeclarar a mesma variável mais de uma vez:

```
let a = 1
let a = 2
```

ou você receberá um erro "declaração duplicada".

Meu conselho é sempre usar *const* e usar *let* somente quando souber que precisará atribuir um valor a essa variável. Por quê? Porque quanto menos poder o nosso código tiver, melhor. Se sabemos que um valor não pode ser reatribuído, é uma fonte a menos para erros.

Agora que vimos como trabalhar com const e let, quero mencionar *var*.

Até 2015, *var* era a única maneira de declarar uma variável em JavaScript. Hoje, uma base de código moderna provavelmente usará const e let. Existem algumas diferenças fundamentais que detalho [neste post](https://flaviocopes.com/javascript-difference-let-var/), mas se você está apenas começando, pode não se importar com elas. Basta usar const e let.

# Tipos

Variáveis ​​em JavaScript não têm nenhum tipo anexado.

Eles não são digitados.

Depois de atribuir um valor com algum tipo a uma variável, você poderá posteriormente reatribuir a variável para hospedar um valor de qualquer outro tipo sem problemas.

Em JavaScript, temos 2 tipos principais de tipos: tipos primitivos e tipos de objetos.

## Tipos primitivos

Os tipos primitivos são:
- numbers
- strings
- booleans
- symbols

E dois tipos especiais: *null* e *undefined*.

## Objetos

Qualquer valor que não é um tipo primitivo (um string, um number, um boolean, null ou undefined) é um objeto.

Os objetos têm propriedades e também métodos que podem atuar nessas propriedades.

Falaremos sobre objetos mais tarde.

# Expressões

Uma expressão é uma única unidade de código JavaScript que o mecanismo JavaScript pode avaliar e retornar um valor.

Expressões podem variar em complexidade.

Começamos pelos muito simples, chamados expressões primárias:

```
2
0.02
'something'
true
false
this // o escopo atual
undefined
i // onde i é uma variávelou uma constante
```

Expressões aritméticas são expressões que recebem uma variável e um operador (falaremos mais sobre operadores em breve) e resultam em um número:

```
1 / 2
i++
i -= 2
i * 2
```

Expressões de string são expressões que resultam em uma string:
```
'A ' + 'string'
```

Expressões lógicas usam operadores lógicos e resolvem para um valor booleano:
```
a && b // a e b
a || b // a ou b
!a // diferente de a
```
Expressões mais avançadas envolvem objetos, funções e arrays, e eu as apresentarei mais tarde.

# Operadores

Os operadores permitem obter duas expressões simples e combiná-las para formar uma expressão mais complexa.

Podemos classificar operadores com base nos operandos com os quais trabalham. Alguns operadores trabalham com 1 operando. A maioria trabalha com 2 operandos. Apenas um operador trabalha com 3 operandos.

Nesta primeira introdução aos operadores, apresentaremos os operadores com os quais você provavelmente está familiarizado: operadores com 2 operandos.

Eu já apresentei um ao falar sobre variáveis: o operador de atribuição <kbg>=</kbg> . Você usa = para atribuir um valor a uma variável:
```
let b = 0
```

Vamos agora apresentar outro conjunto de operadores binários com os quais, pela matemática básica, você já está familiarizado.

## Operador de adição (+)
```
const tres = 1 + 2
const quatro = tres + 1
```

O operador + também faz concatenação de strings se você usar strings, portanto, preste atenção:
```
const tres = 1 + 2
tres + 1 // 4
'tres' + 1 // tres1
```
## Operador de subtração (-)
```
const dois = 4 - 2
```

## Operador de divisão (/)

Retorna o quociente do primeiro operador e do segundo:
```
const resultado = 20 / 5 //result === 4
const resultado = 20 / 7 //result === 2.857142857142857
```

Se você dividir por zero, o JavaScript não gera nenhum erro, mas retorna o valor Infinity (ou -Infinity, se o valor for negativo).
```
1 / 0 //Infinity
-1 / 0 //-Infinity
```

# Operador restante (%)

O restante é um cálculo muito útil em muitos casos:
```
const resultado = 20 % 5 //resultado === 0
const resultado = 20 % 7 //resultado === 6
```
Um restante por zero é sempre NaN, um valor especial que significa "Não é um número":
```
1 % 0 //NaN
-1 % 0 //NaN
```

# Operador de multiplicação (*)

Multiplique dois números
```
1 % 0 //NaN
-1 % 0 //NaN
```
# Operador exponencial (**)

Eleve o primeiro operando à potência do segundo:
```
1 ** 2 //1
2 ** 1 //2
2 ** 2 //4
2 ** 8 //256
8 ** 2 //64
```


