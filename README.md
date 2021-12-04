> # Exercícios Resolvidos - Javascript (Iniciante)


### Índice

+ [Exercícios](#exercícios)
+ [Exercícios com manipulação do DOM](#exercícios-com-manipulação-do-dom) (A incluir)
+ [Resoluções](#resoluções)

<br>

### Atenção! Tente várias vezes antes de olhar as resoluções! ⚠️  

<br>
<br>

> ## Exercícios

1. [Usando o For, imprima no console a frase 'Estou aprendendo Javascript' 10 vezes](#questão-1). 

2. [Crie um array de números, e imprima no console apenas os números ímpares](#questão-2).
 
3. [Crie um array de números (positivos e negativos). Você deve retornar a soma dos números positivos do mesmo](#questão-3).
 
4. [Crie uma string com alguns espaços vazios, depois remova os espaços e imprima no console a nova string](#questão-4).

5. [Faça um script que pede duas notas de um aluno. Em seguida ele deve calcular a média do aluno e dar o seguinte resultado:](#questão-5)

   + A mensagem "Aprovado", se a média alcançada for maior ou igual a sete;
   + A mensagem "Reprovado", se a média for menor do que sete;
   + A mensagem "Aprovado com Distinção", se a média for igual a dez.

6. [Escreva um programa que leia no prompt o nome e um número identificador de um funcionário, seu número de horas trabalhadas, o valor que recebe por hora e calcula o salário desse funcionário. A seguir, mostre o número e o salário do funcionário.](#questão-6)

7. [Imprimir no console os números impares menores que 100.](#questão-7)

8. [Imprimir a tabuada do número 8 no console.](#questão-8)

9. [Calcular a soma dos números impares maiores que 10 e menores que 30.](#questão-9)

10. [Calcular a soma dos números de um array.](#questão-10)

11. [Calcular a média de todos os números de um array ](#questão-11)

12. [Dado o array numeros = [2, 4, 4], crie um programa que o percorra e faça o quadrado de cada elemento, e imprima no console a soma destes quadrados.](#questão-12)

<br />
<br />

### Atenção! Tente várias vezes antes de olhar as resoluções! ⚠️  

<br />
<br />

> # Resoluções

### Questão 1

```javascript
for (i = 0; i < 10; i++) {
  console.log('Estou aprendendo Javascript', i)
}
```
<br>

### Questão 2

```javascript
var novoArray = [2, 4, 7, 5, 3, 12]

for (i = 0; i < novoArray.length; i++) {
  if (!(novoArray[i] % 2 === 0)) {
    console.log(novoArray[i])
  }
}
```

<br>

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

<br>

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

<br>

### Questão 5

```javascript
function media(){
     let nota1 = parseFloat(document.getElementById("nota1").value);
     let nota2 = parseFloat(document.getElementById("nota2").value);

     let media = (nota1 + nota2)/2 ;

     if(media >= 7)
      if(media==10)
       alert("Uau! Aprovado com distinção");
      else
       alert("Parabéns, aprovado! Media "+media);
     else
      alert("Reprovado!")

    }
```

<br>

### Questão 6

```javascript
var id = parseInt(prompt('Informar ID do funcionário: '))

var nome = prompt('Informar nome do funcionário: ')

var horasTrabalhadas = prompt('Informar quantas horas trabalhadas: ')

var valorHora = prompt('Informar o valor da hora: ')

var salario = horasTrabalhadas * valorHora

console.log(
  'O funcionário ' +
    nome +
    ' de ID: ' +
    id +
    ' receberá salario de R$ ' +
    salario
)
```

<br>

### Questão 7

```javascript
for (var i = 1; i <= 100; i += 2) {
 console.log(i);
} 
```

<br>

### Questão 8

```javascript
for (var i = 1; i <= 10; i++) {
 var num = "8 * " + i + " = " + 8 * i;
 console.log(num);
} 
```

<br>

### Questão 9

```javascript
var soma = 0;
for(var i = 11; i <= 30; i += 2) {
 soma += i;
}
console.log(soma); 
```

<br>

### Questão 10

```javascript
function somarArray(ar){
 var soma = 0;
 for (var i = 0; i < ar.length; i++) {
 soma += ar[i];
 }
 return soma;
}
var ar = [2, 3, -1, 5, 7, 9, 10, 15, 95];
var soma = somarArray(ar);
console.log(soma);
```

<br>

### Questão 11

```javascript
function mediaArray(ar) {
 var n = ar.length;
 var soma = 0;
 for (var i = 0; i < n; i++) {
 soma += ar[i];
 }
 return soma / n;
}
var ar = [1, 3, 9, 15, 90];
var media = mediaArray(ar);
console.log("mediaArray: ", media); 
```

<br>

### Questão 12

```javascript
numeros = [2, 4, 4]
var somaQuadrados = 0

for (var i = 0; i < numeros.length; i++) {
  somaQuadrados = somaQuadrados + numeros[i] ** 2
}
console.log(somaQuadrados)
```

<br>
