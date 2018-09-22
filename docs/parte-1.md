# Parte 1

Contato inicial a fim de identificar os objetivos da aluna e sua familiaridade com programação em geral.

## A ver

* variáveis
* constantes
* conversões
* estruturas de controle
* estruturas de repetição
* array e funções

**Tipos:**

* Integer
* Float
* String
* Constante
* Variável

## Variáveis

```javascript
// old ES5 way
var firstName = 'Yuri';

// new ES6+ way
let lastName = 'Doe';
const favoriteFood = 'Guacamole';
const alwaysStartLowerCase = 'Yes!';
```

## Strings

```javascript
const dog = 'totó';
```

## Números

```javascript
const answer = 42;
const negative = -13;
const inf = Infinity;
```

## Booleans

```js
const iLoveJavascript = true;
```

## Operações matemáticas

```js
// mais do mesmo..
1 + 1 = 2
2 * 2 = 4
2 - 2 = 0
2 / 2 = 1

// % - operador resto ou módulo
21 % 5 = 1;
21 % 6 = 3;
21 % 7 = 0;
```

## Objetos globais e métodos

```js
// potência - pow!
Math.pow(2,2) = 4;
Math.pow(3,2) = 9;
Math.pow(3,3) = 27;
Math.pow(-7, 0.5) = NaN // not a number!

// round, floor, ceil
Math.round(6.5) = 7;
Math.round(6.45) = 6;
Math.floor(6.999) = 6;
Math.ceil(6.0001) = 7;
```

## Comprimento

```js
const cat = 'Kitty Kat';
console.log(cat.length);
```

## (básico de) Funções

```js

function f(x) {
  // ...
}

function logsHello() {
  console.log('hello');
}

// usando uma função
logsHello();

// uma função com argumentos
function logsHello(name) {
  console.log('Hello, ' + name);
}

logsHello('Ingrid');

// uma função com múltiplos argumentos
function add(a, b) {
  const sum = a + b;
  return sum;
}

add(1, 5); // 6
```

## Retorno e escopo de função

```js
function dividesTwoNumbers(a, b) { // escopo começa aqui
  const product = a / b;
  return product;
} // escopo termina aqui

dividesTwoNumbers(6, 3); // 2
console.log(product); // undefined
// variável product não existe fora do escopo da função


// uma variável que recebe o retorno da função
function subtractsTwoNumbers(a, b) {
  const difference = a - b;
  return difference;
}

const differenceValue = subtractsTwoNumbers(10, 9);
console.log(differenceValue); // 1
console.log(difference); // undefined
```

## Estruturas de controle

```js
function canDrive(age) {
  if (age > 18) {
    return true;
  }

  return false;
}

canDrive(16); // false
```

## Comparadores

```js
1 < 2
5 <= 5
'Olá'.length > 'Hello'.length
'123' >= '123'
'dog' === 'Dog'
'dog' === 'dog'
2 === '2'
2 === 2
2 == 2
2 == '2'
2 !== '2'
3 !== 3
```