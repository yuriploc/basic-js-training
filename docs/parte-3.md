## Listas / Arrays

```js
// definindo um array
let studentsNames = ['Dan', 'Maria', 'Sara', 'Raj'];

// imprimindo comprimento de um array
console.log(studentNames.length);  // 4

// acessando o índice de um array
console.log(studentNames[1]);  // 'Maria'

// acessando o último item de um array
studentsNames = ['Dan', 'Maria', 'Sara', ... ,'Raj'];

console.log(studentNames[studentNames.length - 1]);  // 'Raj'

// remodelando um array
const studentsNames = ['Dan', 'Maria', 'Sara', 'Raj'];

studentNames[0] = 'João';

console.log(studentNames);  // ['João', 'Maria', 'Sara', 'Raj']
```

### .push & .pop

`.push` insere no início da lista

```js
const studentsNames = ['Dan', 'Maria', 'Sara', 'Raj'];

studentNames.push('Ryan');

console.log(studentNames);  // ['Dan', 'Maria', 'Sara', 'Raj', 'Ryan']
```

e `.pop` remove do final da lista
```js
const studentsNames = ['Dan', 'Maria', 'Sara', 'Raj'];

studentNames.pop();

console.log(studentNames);  // ['Dan', 'Maria', 'Sara']
```

### .unshift & .shift

```js
const studentsNames = ['Dan', 'Maria', 'Sara', 'Raj'];

studentNames.unshift('Ryan');

console.log(studentNames);  // ['Ryan', 'Dan', 'Maria', 'Sara', 'Raj']

studentNames.shift();

console.log(studentNames);  // ['Dan', 'Maria', 'Sara', 'Raj']
```

### Iterando em um array

```js
const studentsNames = ['Dan', 'Maria', 'Sara', 'Raj'];

for (let i = 0; i < studentNames.length; i++) {
  console.log(studentNames[i]);
}
```

### .slice

```js
const animals = ['ant', 'bison', 'camel', 'duck', 'elephant'];
const newAnimals = animals.slice(2); // ["camel", "duck", "elephant"]
```
### .splice

```js
const months = ['Jan', 'March', 'April', 'June'];
months.splice(1, 0, 'Feb');
```

### .map

### .filter

### .sort

## Resumindo

```javascript
// lista vazia
let x = []

// lista com uns valores
let y = [1,2,3]

// adicionar no final da lista
y.push(4)

// adicionar no começo da lista
y.unshift(0)

// remover do final da lista
y.pop() // retorna 4

// remover do começo da lista
y.shift() // retorna 0

// remover de uma posição específica
y = y.splice(1,1) // [1, 3]

// adicionar
y = y.splice(1,0,'x') // [1, "x", 3]

// map, filter, sort
y = y.map(e => 'a' + e) // ['a1','ax','a3']
x = [1,2,3,4,5,6,7,8,9]
x = x.filter(e => e > 5) // [6, 7, 8, 9]
x = x.sort((a,b) => b - a ) // [9, 8, 7, 6]

for(let k in x) console.log("%s: %s", k, x)

```