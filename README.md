> <h1>Exercícios Resolvidos - Javascript (Iniciante)</h1>
<br />

> # Enunciados
<br>

1. [Usando o For, imprima no console a frase 'Estou aprendendo Javascript' 10 vezes](#questão-1). 

2. [Crie um array de números, e imprima no console apenas os números ímpares](#questão-1).
 
3. [Crie um array de números (positivos e negativos). Você deve retornar a soma dos números positivos do mesmo](#questão-1).
 
4. [Crie uma string com alguns espaços vazios, depois remova os espaços e imprima no console a nova string](#questão-1).


<br />
<br />
<br />
<br />
<br />

> # Resoluções
### Questão 1

```javascript
for (i = 0; i < 10; i++) {
  console.log('Estou aprendendo Javascript', i)
}
```

### Questão 2

```javascript
var novoArray = [2, 4, 7, 5, 3, 12]

for (i = 0; i < novoArray.length; i++) {
  if (!(novoArray[i] % 2 === 0)) {
    console.log(novoArray[i])
  }
}
```

### Questão 3

```javascript
arr = [1, -4, 7, 12]
var soma = 0

for (i = 0; i < arr.length; i++) {
  if (arr[i] >= 0) {
    soma = soma + arr[i]
  }
}

console.log(soma)
```

### Questão 4

```javascript
firstString = 'do re mi fa sol la si'
newString = ''

for (i = 0; i < firstString.length; i++) {
  if (firstString[i] !== ' ') {
    newString = newString + firstString[i]
  }
}

console.log(newString)
```




