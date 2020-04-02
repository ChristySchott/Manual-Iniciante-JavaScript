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
20. [Métodos do objeto]()
21. [Classes]()
22. [Herança]()
23. [Programação assíncrona e callbacks]()
24. [Promises]()
25. [Async and Await]()
26. [Escopo de variáveis]()
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

Variáveis em JavaScript não têm nenhum tipo anexado.

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

## Operador restante (%)

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

## Operador de multiplicação (*)

Multiplique dois números
```
1 % 0 //NaN
-1 % 0 //NaN
```
## Operador exponencial (**)

Eleve o primeiro operando à potência do segundo:
```
1 ** 2 //1
2 ** 1 //2
2 ** 2 //4
2 ** 8 //256
8 ** 2 //64
```
# Regras de precedência

Toda declaração complexa com vários operadores na mesma linha apresentará problemas de precedência.

Veja este exemplo:
```
let a = 1 * 2 + 5 / 2 % 2
```

O resultado é 2,5, mas por quê?

Quais operações são executadas primeiro e quais precisam esperar?

Algumas operações têm mais precedência que as outras. As regras de precedência estão listadas nesta tabela:

| Operador |       Descrição       |
| -------- | --------------------- |
|  * / %   | multiplicação/divisão |
|   + -    |    adição/subtração   |
|    =     |         igual         |

Operações no mesmo nível (como + e -) são executadas na ordem em que são encontradas, da esquerda para a direita.

Seguindo estas regras, a operação acima pode ser resolvida desta maneira:
```
let a = 1 * 2 + 5 / 2 % 2
let a = 2 + 5 / 2 % 2
let a = 2 + 2.5 % 2
let a = 2 + 0.5
let a = 2.5
```

# Operadores de comparação

Após os operadores de atribuição e matemáticos, o terceiro conjunto de operadores que quero introduzir são operadores condicionais.

Você pode usar os seguintes operadores para comparar dois números ou duas cadeias.

Os operadores de comparação sempre retornam um boolean, um valor <kbg>true</kbg> ou <kbg>false</kbg>.

Esses são operadores de comparação de desigualdade:

- < significa "menor que"
- <= significa "menor ou igual a"
- '>' significa "maior que"
- '>=' significa "maior ou igual a"

Exemplo:
```
let a = 2
a >= 1 //true
```
Além desses, temos 4 operadores de igualdade. Eles aceitam dois valores e retornam um boolean:

- === checa a igualdade
- !== checa a desiguldade

Observe que também temos <kbg>==</kbg> e <kbg>!=</kbg> em JavaScript, mas eu sugiro usar apenas <kbg>===</kbg> e <kbg>!==</kbg> porque eles podem evitar alguns problemas sutis.

# Condicionais

Com os operadores de comparação instalados, podemos falar sobre condicionais.

Uma instrução <kbg>if</kbg> é usada para fazer o programa seguir uma rota ou outra, dependendo do resultado de uma avaliação de expressão.

Este é o exemplo mais simples, que sempre executa:

```
if (true) {
  //faço algo
}
```
pelo contrário, isso nunca é executado:
```
if (false) {
  //faço algo (? nunca ?)
}
```

O condicional verifica a expressão que você passa para um valor verdadeiro ou falso. Se você passa um número, ele sempre é avaliado como true, a menos que seja 0. Se você passa uma String, ele sempre é avaliado como true, a menos que seja uma String vazia. Essas são regras gerais de conversão de tipos para um booleano.

Você notou as chaves? Isso é chamado de bloco e é usado para agrupar uma lista de instruções diferentes.

Um bloco pode ser colocado onde quer que você possa ter uma única declaração. E se você tiver uma única instrução para executar após as condicionais, poderá omitir o bloco e simplesmente escrever a instrução:

```
if (true) facaAlgo()
```

Mas eu sempre gosto de usar chaves para ficar mais claro.

Você pode fornecer uma segunda parte para a instrução <kbg>if</kbg>: <kbg>else</kbg>.

Você anexa uma instrução que será executada se a condição if for falsa:
```
if (true) {
  //do something
} else {
  //do something else
}
```

Como <kbg>else</kbg> aceita uma instrução, você pode aninhar outra instrução if / else dentro dela:

```
if (a === true) {
  //faca algo
} else if (b === true) {
  //faca algo
} else {
  // faca algo
}
```
# Arrays

Um array é uma coleção de elementos.

Arrays em JavaScript não são um tipo por si só.

Arrays são **objetos**.

Podemos inicializar um array vazio dessas 2 maneiras diferentes:
```
const a = []
const a = Array()
```
O primeirousa a sintaxe literal do Array. O segundo usa a função interna Array.

Você pode preencher previamente a matriz usando esta sintaxe:

```
const a = [1, 2, 3]
const a = Array.of(1, 2, 3)
```

Uma matriz pode conter qualquer valor, mesmo valores de diferentes tipos:
```
const a = [1, 'Flavio', ['a', 'b']]
```
Como podemos adicionar um array a um aray, podemos criar arrays multidimensionais, que têm aplicações muito úteis (por exemplo, um array):

```
const matrix = [
  [1, 2, 3],
  [4, 5, 6],
  [7, 8, 9]
]

matrix[0][0] //1
matrix[2][0] //7
```

Você pode acessar qualquer elemento da matriz referenciando seu índice, que começa do zero:
```
a[0] //1
a[1] //2
a[2] //3
```

Você pode inicializar um novo array com um conjunto de valores usando esta sintaxe, que primeiro inicializa um array de 12 elementos e preenche cada elemento com o número 0:
```
Array(12).fill(0)
```

Você pode obter o número de elementos do array verificando sua propriedade length:
```
const a = [1, 2, 3]
a.length //3
```

Observe que você pode definir o comprimento do array. Se você atribuir um número maior que a capacidade atual dos arrays, nada acontecerá. Se você atribuir um número menor,  o aray será cortado nessa posição:
```
const a = [1, 2, 3]
a //[ 1, 2, 3 ]
a.length = 2
a //[ 1, 2 ]

```

## Como adicionar um item no Array

Nós podemos adicionar um elemento no array com o método <kbg>push()</kbg>:
```
a.push(4)
```

Nós podemos adicionar um elemento no inicio do array utilizando o <kbg>unshift()<kbg>:
```
a.unshift(0)
a.unshift(-2, -1)
```
  
  ## Como remover um item do Array

Nós podemos adicionar um elemento no array com o método <kbg>pop()</kbg>:
```
a.pop()
```

Nós podemos adicionar um elemento no inicio do array utilizando o <kbg>shift()<kbg>:
```
a.shift(0)
```
  
## Como juntar dois ou mais arrays

Nós podemos juntar arrays com o método <kbg>concat()</kbg>:
```
const a = [1, 2]
const b = [3, 4]
const c = a.concat(b) //[1,2,3,4]
a //[1,2]
b //[3,4]
```

Nós também podemos utilizar o operador *spread* <kbg>(...)</kbg>, desse modo:
```
const a = [1, 2]
const b = [3, 4]
const c = [...a, ...b]
c //[1,2,3,4]
```

Nós podemos adicionar um elemento no inicio do array utilizando o <kbg>unshift()<kbg>:
```
a.unshift(0)
a.unshift(-2, -1)
```
  
   ## Como encontrar um item no Array

Nós podemos usar o método <kbg>find()</kbg> num array:
```
a.find((element, index, array) => {
  //return true or false
})

```

Retorna o primeiro item que retorna true e retorna undefined se o elemento não for encontrado.

Uma sintaxe comumente usada é:

```
a.find(x => x.id === my_id)

```

A linha acima retornará o primeiro elemento no array que possui id === my_id.

findIndex () funciona de maneira semelhante a find (), mas retorna o índice do primeiro item que retorna true e, se não for encontrado, retorna undefined:

```
a.findIndex((element, index, array) => {
  //return true or false
})
```
 Outro método é o <kbg>includes()</kbg>
 
```
a.includes(value) 
```
Retorna *true* se <kbg>a</kbg> contém <kbg>value</kbg>.


```
a.includes(value, i)
```
Retorna *true* se <kbg>a</kbg> contém <kbg>value</kbg> depois da posição <kbg>i</kbg>.

# Strings

Uma string é uma sequência de caracteres.

Também pode ser definido como uma string literal, entre aspas ou aspas duplas:

```
'Uma string'
"Outra string"
```
Pessoalmente, prefiro aspas simples e uso aspas duplas apenas em HTML para definir atributos.

Você atribui um valor de string a uma variável assim:
```
const nome = 'Flavio'
```
Você pode determinar o comprimento de uma string usando a propriedade length:
```
'Flavio'.length //6
const nome = 'Flavio'
nome.length //6
```

Esta é uma string vazia: ''. Sua propriedade length é 0:
```
''.length() //0
```

Duas strings podem ser unidas utilizando o operador <kbg>+</kbg>.

```
'Uma' + 'String' // UmaString
```

Duas variáveis podem ser unidas utilizando o operador <kbg>+</kbg>.
```
const nome = 'Flavio'
"Meu nome é " + nome //Meu nome é Flavio
```
Outra maneira de definir strings é usar literais de modelo (template literals), definidos dentro de acentos graves (<kbg>``</kbg). Eles são especialmente úteis para tornar as strings multilinhas muito mais simples. Com aspas simples ou duplas, você não pode definir facilmente uma string de múltiplas linhas - você precisará usar caracteres de escape.
  
 Depois que um template literal é aberto com o acento grave, basta pressionar enter para criar uma nova linha, sem caracteres especiais, e ela é renderizada como é escrita:
 ```
 const string = `Oi
essa

string
é incrivel!`
 ```
 
 Eles também são ótimos pelo fato de fornecerem uma maneira fácil de interpolar variáveis e expressões em seqüências de caracteres.
 ```
 const var = 'test'
const string = `something ${var}` 
//something test
 ```
 
 dentro do $ {} você pode adicionar qualquer coisa, até expressões:
 
```
const string = `something ${1 + 2 + 3}`
const string2 = `something 
  ${foo() ? 'x' : 'y'}` 
```

# Loops

Os loops são uma das principais estruturas de controle do JavaScript.

Com um loop, podemos automatizar e repetir um bloco de código quantas vezes quisermos que ele seja executado, mesmo que indefinidamente.

O JavaScript fornece vários modos de percorrer loops.

Eu quero focar em 3 modos:

- while loops
- for loops
- for..of loops

## while 

O loop while é a estrutura de loop mais simples que o JavaScript nos fornece.

Adicionamos uma condição após a palavra-chave while e fornecemos um bloco que é executado até que a condição seja avaliada como verdadeira.

Exemplo:
```
const list = ['a', 'b', 'c']
let i = 0
while (i < list.length) {
  console.log(list[i]) //valor
  console.log(i) //index
  i = i + 1
}
```
Você pode interromper um loop while usando a palavra-chave break, assim:
```
while (true) {
  if (somethingIsTrue) break
}
```

e se você decidir que, no meio de um loop, deseja pular a iteração atual, poderá pular para a próxima usando continue:

```
while (true) {
  if (somethingIsTrue) continue

  //do something else
}

```

Muito parecido com while, nós temos os loops **do.. while**. É basicamente a mesma coisa que o while, exceto que a condição é avaliada após a execução do bloco de código.

Isso significa que o bloco é sempre executado pelo menos uma vez.

Exemplo:
```
const list = ['a', 'b', 'c']
let i = 0
do {
  console.log(list[i]) //valor
  console.log(i) //index
  i = i + 1
} while (i < list.length)
```

## for

A segunda estrutura de loop muito importante no JavaScript é o loop for.

Usamos a palavra-chave for e passamos um conjunto de três instruções: a inicialização, a condição e a parte do incremento.

Exemplo:
```
const list = ['a', 'b', 'c']

for (let i = 0; i < list.length; i++) {
  console.log(list[i]) //value
  console.log(i) //index
}

```

Assim como com os loops while, você pode interromper um loop *for* usando <kbg>break</kbg> e avançar rapidamente para a próxima iteração de um *for usando* <kbg>continue</kbg>.

## for..of

Esse loop é relativamente recente (introduzido em 2015) e é uma versão simplificada do loop for:

```
const list = ['a', 'b', 'c']

for (const value of list) {
  console.log(value) //value
}
```

# Funções

Em qualquer programa JavaScript moderadamente complexo, tudo acontece dentro das funções.

As funções são uma parte essencial e essencial do JavaScript.

O que é uma função?

Uma função é um bloco de código independente.

Aqui está uma declaração de função:

```
function getDado() {
  // faço algo
}
```

Uma função pode ser executada a qualquer momento, invocando-a assim:
```
getDado()
```

Um função pode ter um ou mais argumentos:
```
function getDado() {
  //faço algo
}

function getDado(cor) {
  //faço algo
}

function getDado(cor, idade) {
  //faça algo
}
```

Quando podemos passar um argumento, chamamos a função que passa os parâmetros:
```
function getDado(cor, idade) {
  //faça algo
}

getDado('verde', 24)
getDado('preto')
```
Observe que, na segunda chamada, passei o parâmetro string preto como argumento de cor, mas sem idade. Nesse caso, a idade dentro da função é indefinida.

Podemos verificar se um valor não é indefinido usando esta condicional:
```
function getDado(cor, idade) {
  //faça algo
  if (typeof idade !== 'undefined') {
    //...
  }
}
```
<kbg>typeof</kbg> é um operador unário que nos permite verificar o tipo de uma variável.

Você também pode verificar desta maneira:
```
function getDado(cor, idade) {
  //faça algo
  if (idade) {
    //...
  }
}
```

Embora o condicional também seja verdadeiro se a idade for nula, 0 ou uma sequência vazia.

Você pode ter valores padrão para parâmetros, caso eles não sejam passados:
```
function getDado(cor = 'black', idade = 25) {
  //faça algo
}
```

Você pode passar qualquer valor como parâmetro: numbers, strings, booleans, arrays, objects, e também funções.

Uma função tem um valor de retorno. Por padrão, uma função retorna indefinida, a menos que você adicione uma palavra-chave de retorno com um valor:
```
function getDado() {
  // faça algo
  return 'oi!'
}
```

Podemos atribuir esse valor de retorno a uma variável quando chamamos a função:
```
function getDado() {
  // faça algo
  return 'oi!'
}

let result = getDado()
```
*result* agora possui uma String com o valor "oi!"

Você pode retornar apenas um valor.

Para retornar vários valores, você pode retornar um objeto ou um array assim:
```
function getDado() {
  return ['Flavio', 37]
}

let [nome, idade] = getDado()
```

As funções podem ser definidas dentro de outras funções:
```
const getDado = () => {
  const doSomething = () => {}
  doSomething()
  return 'test'
}
```

A função aninhada não pode ser chamada de fora da função envolvente.

Você também pode retornar uma função de uma função.

# Arrow Functions

As arrow functions (funções de seta) são uma introdução recente ao JavaScript.

Eles são frequentemente usados em vez de funções "regulares", as que descrevi no capítulo anterior. Você encontrará os dois formulários usados em qualquer lugar.

Visualmente, eles permitem escrever funções com uma sintaxe mais curta, de:
```
function getDado(){
 //
}
```
para:

```
() => {
  //...
}
```

Mas .. observe que não temos um nome aqui.

As funções de seta são anônimas. Devemos atribuí-los a uma variável.

Podemos atribuir uma função regular a uma variável, assim:

```
let getDado = function getDado() {
  //...
}
```

Quando fazemos isso, podemos remover o nome da função:

```
let getData = function() {
  //...
}
```
e chamar a função usando o nome da variável:
```
let getDado = function() {
  //...
}
getDado()
```
É a mesma coisa que fazemos com as arrow functions:
```
let getDado = () => {
  //...
}
getDado()
```
Se o corpo da função contiver apenas uma única instrução, você poderá omitir os parênteses e escrever tudo em uma única linha:
```
const getDado = () => console.log('oi!')
```

Os parâmetros são passados entre parênteses: 
```
const getDado = (param1, param2) => 
  console.log(param1, param2)
```

Se você tiver um (e apenas um) parâmetro, poderá omitir completamente os parênteses:
```
const getDado = param => console.log(param)
```

As arrows functions permitem um retorno implícito - os valores são retornados sem a necessidade de usar a palavra-chave *return*.

Funciona quando há uma instrução de uma linha no corpo da função:
```
const getDado = () => 'teste'

getDado() //'teste'
```

Como nas funções regulares, podemos ter valores padrão para parâmetros caso eles não sejam passados:
```
const getDado = (cor = 'preto', 
                 idade = 2) => {
  //do something
}
```

E, como funções regulares, só podemos retornar um valor.

As arrows functions também podem conter outras arrows functions ou até funções regulares.

Os dois tipos de funções são muito semelhantes, então você pode perguntar por que as arrows functions foram introduzidas. A grande diferença com as funções regulares é quando elas são usadas como métodos de objeto. Isso é algo que analisaremos em breve.

# Objetos

Qualquer valor que não é um tipo primitivo (uma string, um number, um boolean, um symbol, null, ou undefined) é um objeto.

Aqui está como definimos um objeto:

```
const car = {

}
```
Essa é a sintaxe literal do objeto, que é uma das coisas mais agradáveis do JavaScript.

Você também pode usar a sintaxe <kbg> new Object() </kbg>:
```
const car = new Object()
```
Outra sintaxe é a <kbg> Object.create() </kbg>.
```
const car = Object.create()
```
Você também pode inicializar um objeto usando a palavra-chave <kbg>new</kbg> antes de uma função com letra maiúscula. Esta função serve como um construtor para esse objeto. Lá, podemos inicializar os argumentos que recebemos como parâmetros, para configurar o estado inicial do objeto:
```
function Car(marca, modelo) {
  this.marca = marca
  this.modelo = modelo
}
```

Nós podemos inicia um objeto usando:
```
const meuCarro = new Car('Ford', 'Fiesta')
meuCarro.marca//'Ford'
meuCarro.modelo //'Fiesta'
```
Os objetos são sempre passados ​​por referência.

Se você atribuir a uma variável o mesmo valor de outra, se for um tipo primitivo como um número ou uma sequência, eles serão passados por valor.

Veja este exemplo:

```
let idade = 36
let minhaIdade = age
minhaIdade = 37
idade //36
```

```
const carro = {
  cor: 'azul'
}
const outroCarro = carro
outroCarro.cor = 'amarelo'
carro.cor //'amarelo'
```
Mesmo arrays ou funções são objetos ocultos, por isso é muito importante entender como eles funcionam.

# Propriedades do objeto

Os objetos têm propriedades, compostas por um rótulo associado a um valor.

O valor de uma propriedade pode ser de qualquer tipo, o que significa que pode ser um array, uma função e pode até ser um objeto, pois os objetos podem aninhar outros objetos.

Esta é a sintaxe literal do objeto que vimos no capítulo anterior:
```
const car = {

}
```

Podemos definir uma propriedade <kbg>cor</kbg> desta maneira:
```
const carro = {
  cor: 'azull'
}
```

Aqui temos um objeto de carro com uma propriedade chamada cor, com o valor azul.

Os rótulos podem ser qualquer string, mas cuidado com caracteres especiais - se eu quisesse incluir um caractere inválido como nome de variável no nome da propriedade, teria que usar aspas:
```
const carro = {
  cor: 'azul',
  'a cor': 'azul'
}
```
Caracteres de nome de variável inválidos incluem espaços, hífens e outros caracteres especiais.

Como você pode ver, quando temos várias propriedades, separamos cada propriedade por vírgula.

Podemos recuperar o valor de uma propriedade usando 2 sintaxes diferentes.

A primeira é a notação de ponto:
```
carro.cor //'azul'
```
O segundo (que é o único que podemos usar para propriedades com nomes inválidos), é usar colchetes:
```
carro['a cor'] //'azul'
```

Se você acessar uma propriedade inexistente, obterá o valor indefinido:
```
carro.marca //undefined
```
Como mencionado anteriormente, os objetos podem ter objetos aninhados como propriedades:
```
const carro = {
  marca: {
    nome: 'Ford'
  },
  cor: 'azul'
}

```

Neste exemplo, você pode acessar o nome da marca usando:

```
carro.marca.nome
```
ou

```
carro['marca']['nome']
```

Você pode definir o valor de uma propriedade ao definir o objeto.

Mas você sempre pode atualizá-lo mais tarde:

```
const carro = {
  cor: 'azul'
}

carro.cor = 'amarelo'
carro['cor'] = 'vermelho'
```

E você também pode adicionar novas propriedades a um objeto:
```
carro.modelo = 'Festa'

carro.modelo // 'Fiesta'
```
Dado o objeto
```
const carro = {
  cor: 'azul',
  marca: 'Ford'
}
```

você pode excluir uma propriedade desse objeto usando

```
delete carro.marca
```
# Métodos de objetos 

Eu falei sobre funções em um capítulo anterior.

As funções podem ser atribuídas a uma propriedade de função e, nesse caso, são chamadas de métodos.

Neste exemplo, a propriedade <kbg>start</kbg> possui uma função atribuída, e podemos invocá-la usando a sintaxe do ponto que usamos para propriedades, com os parênteses no final:

```
const carro = {
  marca: 'Ford',
  modelo: 'Fiesta',
  start: function() {
    console.log('Started')
  }
}

carro.start()
```

Dentro de um método definido usando a sintaxe <kbg>function () {}</kbg>, temos acesso à instância do objeto fazendo referência a <kbg>this</kbg>.

No exemplo a seguir, temos acesso aos valores das propriedades de <kbg>marca</kbg> e <kbg>modelo</kbg> usando <kbg>this.marca</kbg> e <kbg>this.modelo</kbg>:
```
const car = {
  marca: 'Ford',
  modelo: 'Fiesta',
  start: function() {
    console.log(`Started 
      ${this.marca} ${this.modelo}`)
  }
}

carro.start()
```
É importante observar essa distinção entre funções regulares e arrows functions - não temos acesso a <kbg>this</kbg> se usarmos uma arrow function:
```
const carro = {
  marca: 'Ford',
  modelo: 'Fiesta',
  start: () => {
    console.log(`Started 
      ${this.marca} ${this.modelo}`) // não irá funcionar
  }
}

carro.start()
```
Isso ocorre porque as arrows functions não estão vinculadas ao objeto.

Essa é a razão pela qual funções regulares são frequentemente usadas como métodos de objeto.

Os métodos podem aceitar parâmetros, como funções regulares:
```
const carro = {
  marca: 'Ford',
  modelo: 'Fiesta',
  vaiPara: function(destino) {
    console.log(`Indo para ${destino}`)
  }
}

carro.vaiPara('Roma')
```
# Classes 

Conversamos sobre objetos, que são uma das partes mais interessantes do JavaScript.

Neste capítulo, subiremos um nível introduzindo classes.

O que são classes? Eles são uma maneira de definir um padrão comum para vários objetos.

Vamos pegar um objeto de pessoa:
```
const pessoa = {
  nome: 'Flavio'
}
```

Podemos criar uma classe chamada <kbg>Pessoa</kbg> (observe a letra <kbg>P</kbg> maiúscula, uma convenção ao usar classes), que possui uma propriedade <kbg>nome</kbg>:
```
class Pessoa {
  nome
}
```

Agora, a partir desta classe, inicializamos um objeto <kbg>flavio</kbg> como este:
```
const flavio = new Pessoa()
```
<kbg>flavio</kbg> é chamado uma instância da classe <kbg>Pessoa</kbg>.

Podemos definir o valor da propriedade <kbg>nome</kbg>:
```
flavio.nome = 'Flavio'
```

e podemos acessar isso usando

```
flavio.nome
```

como fazemos para as propriedades do objeto.

As classes podem conter propriedades, como nome e métodos.

Os métodos são definidos desta maneira:
```
class Pessoa {
  ola() {
    return 'Oi, eu sou o Flavio'
  }
}
```
e podemos invocar métodos em uma instância da classe:
```
class Pessoa {
  ola() {
    return 'Oi, eu sou o Flavio'
  }
}
const flavio = new Pessoa()
flavio.ola()
```

Existe um método especial chamado <kbg>constructor()</kbg> que podemos usar para inicializar as propriedades da classe quando criamos uma nova instância de objeto.

Funciona assim:
```
class Pessoa {
  constructor(nome) {
    this.nome = nome
  }

  ola() {
    return 'Ola, eu me chamo ' + this.nome + '.'
  }
}
```
Observe como usamos <kbg>this</kbg> para acessar a instância do objeto.

Agora podemos instanciar um novo objeto da classe, passar uma string e, quando chamarmos <kbg>ola</kbg>, receberemos uma mensagem personalizada:
```
const flavio = new Pessoa('flavio')
flavio.ola() //'Ola, eu sou flavio.'
```

Quando o objeto é inicializado, o método construtor é chamado com todos os parâmetros passados.

Normalmente, os métodos são definidos na instância do objeto, não na classe.

Você pode definir um método como <kbg>static</kbg> para permitir que ele seja executado na classe:

```
class Pessoa {
  static olaGenerico() {
    return 'Olá'
  }
}

Pessoa.olaGenerico() //Olá
```

Isso é muito útil as vezes.

# Herança

Uma classe pode **estender** outra classe e os objetos inicializados usando essa classe herdam todos os métodos de ambas as classes.

Suponha que tenhamos uma classe <kbg>Pessoa</kbg>:
```
class Pessoa {
  ola() {
    return 'Olá, eu sou uma Pessoa'
  }
}
```
Podemos definir uma nova classe, <kbg>Programador</kbg>, que estende <kbg>Pessoa</kbg>:
```
class Programador extends Pessoa {

}
```
Agora, se instanciarmos um novo objeto com a classe Programador, ele terá acesso ao método ola ():
```
const flavio = new Programador()
flavio.ola() //'Olá, eu sou uma Pessoa'
```
Dentro de uma classe filho, você pode fazer referência à classe pai chamando  <kbg>super()</kbg>:
```
class Programador extends Pessoa {
  ola() {
    return super.ola() + 
      '. Eu tambem sou um programador.'
  }
}

const flavio = new Programador()
flavio.ola()
```
O programa acima imprime *Olá, eu sou uma Pessoa. Eu também sou um programador.*

# Programação Assícrona e Callbacks

Na maioria das vezes, o código JavaScript é executado de forma síncrona.

Isso significa que uma linha de código é executada, a próxima é executada e assim por diante.

Tudo está como você espera e como funciona na maioria das linguagens de programação.

No entanto, há momentos em que você não pode esperar apenas pela execução de uma linha de código.

Você não pode esperar apenas 2 segundos para carregar um arquivo grande e interromper o programa completamente.

Você não pode simplesmente esperar que um recurso de rede seja baixado antes de fazer outra coisa.

JavaScript resolve esse problema usando callbacks.

Um dos exemplos mais simples de como usar **callbacks** é com temporizadores. Os temporizadores não fazem parte do JavaScript, mas são fornecidos pelo navegador e pelo Node.js. Deixe-me falar sobre um dos temporizadores que temos: <kbg>setTimeout()</kbg>.

A função <kbg>setTimeout()</kbg> aceita 2 argumentos: uma função e um número. O número são os milissegundos que devem passar antes da execução da função.

Exemplo:

```
setTimeout(() => {
  // executa após dois segundos
  console.log('dentro da função')
}, 2000)
```
A função que contém a linha <kbg>console.log('dentro da função')</kbg> será executada após 2 segundos.

Se você adicionar um <kbg>console.log('antes')</kbg> antes da função e <kbg>console.log('antes')</kbg> depois:
```
console.log('antes')
setTimeout(() => {
  // executa após 2 segundos
  console.log('dentro da função')
}, 2000)
console.log('antes')
```

Você verá isso acontecendo no seu console:
```
antes
depois
dentro da função
```

A *callback* é executada assincronamente.

Esse é um padrão muito comum ao trabalhar com o sistema de arquivos, a rede, os eventos ou o DOM no navegador.

Todas as coisas que mencionei não são JavaScript "central", portanto não são explicadas neste manual, mas você encontrará muitos exemplos nos meus outros manuais disponíveis em https://flaviocopes.com.

Veja como podemos implementar callbacks em nosso código.

Definimos uma função que aceita um parâmetro de callback, que é uma função.

Quando o código está pronto para chamar o callback, nós o chamamos passando o resultado:
```
const facaAlgo = callback => {
  //faça algo
  //faça algo
  const resultado = /* .. */
  callback(resultado)
}
```
O código que usa essa função usaria assim:
```
facaAlgo(resultado => {
  console.log(resultado)
})
```
# Promises 

As promessas são uma maneira alternativa de lidar com código assíncrono.

Como vimos no capítulo anterior, com callbacks estaríamos passando uma função para outra chamada de função, que seria chamada quando a função terminasse o processamento.

Como isso:
```
doSomething(resultado => {
  console.log(resultado)
})
```

Quando o código doSomething () termina, chama a função recebida como um parâmetro:

```
const doSomething = callback => {
  //faça algo
  //faça algo
  const resultado = /* .. */
  callback(resultado)
}
```

O principal problema dessa abordagem é que, se precisarmos usar o resultado dessa função no restante do código, todo o código deverá estar aninhado dentro do callback e, se precisarmos fazer 2-3 retornos de chamada, inserimos o que é geralmente definido "callback hell" com muitos níveis de funções recuados em outras funções:
```
facaAlgumaCoisa(resultado => {
  facaAlgumaOutraCoisa(outroResultado => {
     facaAlgumaOutraCoisaDenovo(aindaOutroResultado => {
      console.log(resultado)
    })
  }) 
})
```

Promessas são uma maneira de lidar com isso.

Em vez de fazer:
```
facaAlgo(resultado => {
  console.log(resultado)
})
```
Chamamos uma função baseada em promessa desta maneira:
```
facaAlgo()
  .then(resultado => {
    console.log(resultado)
  })
```

Primeiro chamamos a função, então temos um método <kbg>then()</kbg> chamado quando a função termina.

A identação não importa, mas você costuma usar esse estilo para maior clareza.

É comum detectar erros usando um método <kbg>catch()</kbg>:

```
facaAlgo()
  .then(resultado => {
    console.log(resultado)
  })
  .catch(erro => {
    console.log(erro)
  })
```

Agora, para poder usar essa sintaxe, a implementação da função <kbg>facaAlgo()</kbg> deve ser um pouco especial. Ele deve usar a API Promises.

Em vez de declarar como uma função normal:
```
const facaAlgo = () => {
  
}
```

Nós a declaramos como um objeto promise:
```
const facaAlgo = new Promise()
```
e passamos uma função no construtor Promise:
```
const facaAlgo = new Promise(() => {

})
```

Esta função recebe 2 parâmetros. A primeira é uma função que chamamos para resolver a promessa, a segunda é uma função que chamamos para rejeitar a promessa.
```
const doSomething = new Promise(
  (resolve, reject) => {
    
})
```
Resolver uma promessa significa concluí-la com sucesso (o que resulta em chamar o método <kbg>then()</kbg> em qualquer que seja o uso).

Rejeitar uma promessa significa encerrá-la com um erro (o que resulta em chamar o método <kbg>catch()</kbg> no que quer que seja usado).

Aqui está como:
```
const facaAlgo = new Promise(
  (resolve, reject) => {
    // algum código
    const success = /* ... */
    if (success) {
      resolve('ok')
    } else {
      reject('um erro ocorreu ')
    }
  }
)
```

Podemos passar um parâmetro para as funções de resolução e rejeição, de qualquer tipo que desejar.

# Asinc and Await

As funções assíncronas são uma abstração de nível superior de promessas.

Uma função assíncrona retorna uma promessa, como neste exemplo:
```
const getDado = () => {
  return new Promise((resolve, reject) => {
    setTimeout(() => 
      resolve('algum dado'), 2000)
  })
}
```
Qualquer código que queira usar esta função usará a palavra-chave await antes da função:
```
const dado = await getDado()
```

e, assim, todos os dados retornados pela promessa serão atribuídos à variável de dados.

No nosso caso, os dados são a string "algum dado".

Com uma ressalva específica: sempre que usarmos a palavra-chave await, devemos fazê-lo dentro de uma função definida como assíncrona.

Assim:
```
const facaAlgo = async () => {
  const dado = await getDado()
  console.log(dado)
}
```

A dupla async / await nos permite ter um código mais limpo e um modelo mental simples para trabalhar com código assíncrono.

Como você pode ver no exemplo acima, nosso código parece muito simples. Compare-o ao código usando promessas ou funções de retorno de chamada.

E este é um exemplo muito simples, os principais benefícios surgirão quando o código for muito mais complexo.

Como exemplo, veja como você poderia obter um recurso JSON usando a API Fetch e analisá-lo usando promessas:

```
const getDadoPrimeiroUsuario = () => {
  // pega lista de usuários
  return fetch('/users.json') 
    // parse JSON
    .then(response => response.json()) 
    // pegue primeiro usuário
    .then(users => users[0]) 
    // pegue dado do usuário
    .then(user => 
      fetch(`/users/${user.name}`)) 
    // parse JSON
    .then(userResponse => response.json()) 
}

getDadoPrimeiroUsuario()
```

E aqui está a mesma funcionalidade fornecida usando await / async:
```
const getDadoPrimeiroUsuario = async () => {
  // pega lista de usuários
  const response = await fetch('/users.json') 
  // parse JSON
  const users = await response.json() 
  // pegue primeiro usuário
  const user = users[0] 
  // pega dado do usuário
  const userResponse = 
    await fetch(`/users/${user.name}`)
  // parse JSON
  const userData = await user.json() 
  return userData
}

getDadoPrimeiroUsuario()
```

# Escopo de variáveis

Quando introduzi variáveis, falei sobre o uso de <kbg>const</kbg>, <kbg>let</kbg> e <kbg>var</kbg>.

Escopo é o conjunto de variáveis visíveis para uma parte do programa.

Em JavaScript, temos um escopo global, escopo de bloco e escopo de função.

Se uma variável é definida fora de uma função ou bloco, ela é anexada ao objeto global e possui um escopo global, o que significa que está disponível em todas as partes de um programa.

Há uma diferença muito importante entre as declarações <kbg>var</kbg>, <kbg>let</kbg> e <kbg>const</kbg>.

Uma variável definida como <kbg>var</kbg> dentro de uma função é visível apenas dentro dessa função, semelhante aos argumentos de uma função.

Uma variável definida como <kbg>const</kbg> ou <kbg>let</kbg>, por outro lado, só é visível dentro do bloco em que está definida.

Um bloco é um conjunto de instruções agrupadas em um par de chaves, como as que podemos encontrar dentro de uma instrução if, um loop for ou uma função.

É importante entender que um bloco não define um novo escopo para <kbg>var</kbg>, mas sim para <kbg>let</kbg> e <kbg>const</kbg>.

Isso tem implicações muito práticas.

Suponha que você defina uma variável <kbg>var</kbg> dentro de um if condicional em uma função
```
function getDado() {
  if (true) {
    var dados = 'algum dado'
    console.log(dados) 
  }
}
```
Se você chamar essa função, "alguns dados" será impressos no console.

Se você tentar mover console.log(dados) após o <kbg>if</kbg>, ele ainda funcionará:
```
function getDado() {
  if (true) {
    var dados = 'algum dado'
  }
  console.log(dados) 
}
```
Mas se você alternar <kbg>var dados</kbg> para <kbg>let dados</kbg>:
```
função getDado () {
  if (true) {
    let dados = 'alguns dados'
  }
  console.log (dados)
}
```

Você receberá um erro: **ReferenceError: dados is not defined.**

Isso ocorre porque <kbg>var</kbg> tem escopo de função e algo especial está acontecendo aqui chamado de elevação. Em resumo, a declaração <kbg>var</kbg> é movida para o topo da função mais próxima pelo JavaScript antes de executar o código. É assim que a função se parece com JS internamente, mais ou menos:
```
function getDado() {
  var dados
  if (true) {
    dados = 'alguns dados'
  }
  console.log(dados) 
}
```
É por isso que você também pode colocar <kbg>console.log(dados)</kbg> na parte superior de uma função, mesmo antes de ser declarada, e ficará indefinido como um valor para essa variável:
```
function getDado() {
  console.log(dados) 
  if (true) {
    var dados = 'alguns dados'
  }
}
```

mas se você trocar para <kbg>let</kbg>,você vai receber um erro: **ReferenceError: data is not defined**,  porque o içamento não acontece nas declarações <kbg>let</kbg>.

<kbg>const</kbg> segue as mesmas regras do <kbg>let</kbg>: tem o escopo bloqueado.

Pode ser complicado no começo, mas quando você perceber essa diferença, verá porque o <kbg>var</kbg> é considerado uma prática ruim hoje em dia em comparação com o <kbg>let</kbg> - eles têm menos partes móveis e seu escopo é limitado ao bloco, o que também os torna muito boas como variáveis de loop porque elas deixam de existir após o término de um loop:
```
function doLoop() {
  for (var i = 0; i < 10; i++) {
    console.log(i)
  }
  console.log(i)
}

doLoop()
```

Quando você sai do loop, <kbg>i</kbg> será uma variável válida com o valor 10.

Se você alternar para <kbg>let</kbg>, ao tentar o <kbg>console.log(i)</kbg> resultará em um erro **ReferenceError: i is not defined.**

# Conclusão

Muito obrigado por ler este livro.

Espero que isso inspire você a aprender mais sobre JavaScript.

Para saber mais sobre JavaScript, consulte o meu blog https://flaviocopes.com.
