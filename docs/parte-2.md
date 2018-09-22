# Revisando (e incrementando)

## Tipos de dados

- [ ] Números (ex. 2, 1.5, 3000)
- [ ] Infinito (`Infinity`) **sério**
- [ ] Strings (ex. "azul", 'amarelo', `verde`, `azul ${55}`)
- [ ] Data (ex. `new Date()`)
- [ ] Funções (ex. `const x = a => 2 + a`, `function (z) { return z*z }`)
- [ ] Listas (ex. `[]`, `[1,2,3]`, `["a",'b', new Date(), 4]`)
- [ ] Mapas / Objetos literais (ex. `{}`, `{ a: 1, b: "2" }`)
- [ ] Nulo (`null`)
- [ ] Não-definido (`undefined`) **sério**
- [ ] Não é um número (`NaN`) **sério**
- [ ] Regex (ex. `/.* de .* de [0-9]+/` )
- [ ] Classes (ex. `class Rectangle extends Shape { }` )

## Undefined e null

`undefined` significa que o que você está pedindo não existe

```js
console.log(unkownVar); // undefined
```

`null` é um objeto sem valor associado a ele. Enquanto `undefined` é setado pela própria linguagem, `null` é setado por outro desenvolvedor ou seu própio código.

```js
let phoneNumber = '123-456-7890';
console.log(phoneNumber);
phoneNumber = null;

console.log(phoneNumer); // null
```

## Strings

```javascript
const name = 'Ingrid'
console.log('oi!')
console.log('oi, ' + name + '!')
console.log(`oi!`)
console.log(`oi, ${name}!`)
```

## Objetos / Mapas

```javascript
let m1 = {} // empty object
m1.x = 2 // {x: 2}

let m2 = { a:1, b:2 }
m2.c = 3 // {a: 1, b: 2, c: 3}

for(let k in m2) {
  console.log("%s: %s", k, m2[k])
}

// tem isso aqui também, complicaremos na próxima parte.

const usuario = {
  nome: 'Yuri',
  list() {
    return [1,2,3]
  },
  identificador: "XDFGgjhJFffgdg"
}
```

## Funções

```javascript
// funções
function f(x) {
  return x + 1
}

// clássica
function a(b, c, d) {
  console.log(c)
  return b + d
}

// arrow function
const f = (x) => {
  return x + 1
}

// happy arrow
const a = (b, c, d) => {
  console.log(c)
  return  b + d
}

// arrow function reduzida
const e = (f,g) => f + g

const f = x => x + 1

// funções que tenham uma linha usam esse corpo como o prórpio retorno

const b = (c,d) => {
  return c + d
}

// funções com um só parâmetro dispensam os parênteses
const b = c => c * c
b(4) // usando a função
// imprime 16

// funções dentro de mapas tem direito a sintaxe especial:
const obj = {
  myfun(){ return 'something' }
}
```

## Estruturas de Controle

```javascript
// if
let i = 0

if (i >= 0) {
  console.log('Oi, Ingrid!')
}

// if-else
const nome = 'Patrícia'

if (nome === 'Joana') {
  console.log(nome + '?')
} else {
  console.log(nome + '!')
}

if (false) {
    console.log('Pula!');
} else if (true) {
    console.log('Roda em 1');
} else if (true) {
    console.log('Não roda :(');
}

// if ternário
const nome = 'Patrícia'

nome === 'Joana' ? console.log(nome + '?') : console.log(nome + '!')

// switch
switch(x) {
  case 1:
    console.log('got one');
    break;

  case 'deer':
    console.log('got baaaa!!!');
    break;

  default:
    return 'end!';
}
```

## Estruturas de repetição

```javascript
// for

// | declare a var | conditional expression | increment var|
for (let i = 0     ; i < 10                 ; i++          ) {
    console.log(i);
}

for(let k = 0; k < 10; k++) {
  console.log(`eu valho ${k}`)
}

// for infinito. Cuidado!
for (let i = 0; i >= 0; i++) {
  console.log(i);
}

// while

let i = 10

while(i-- > 0) {
  console.log('Eu valho '.concat(i))
}

// tem o do-while também

let j = 0;

do {
  console.log('eu valho ' + j )
  j = j + 1
} while(j < 10)

```

## Operações lógicas e matemáticas

```javascript
// and
const a = 5;

if (a !== 2 && a > 0) {
  console.log('número ' + a + 'é maior que zero E diferente de dois')
}

// or
if (a < 0 || a === 5) {
  console.log('número menor que zero OU igual a cinco')
}

// NOT
if (!false) {
  console.log('Falso negado é true, portanto essa mensagem vai aparecer :)');
}

// mod
if (a % 1 === 0) {
  console.log('número ímpar')
} else if (a % 2 === 0) {
  console.log('número par')
} else {
  console.log('nem par nem ímpar?')
}

// Math lib
console.log(Math.PI)
console.log(Math.floor(1.2))
console.log(Math.ceil(3.14))
console.log(-Infinity)
console.log(Infinity)
```