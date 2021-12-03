> <h1>Exercícios Resolvidos - Javascript (Iniciante)</h1>
<br />

> # Enunciados
<br>

1. [Usando o For, imprima no console a frase 'Estou aprendendo Javascript' 10 vezes](#questão-1). 

2. [Crie um array de números, e imprima no console apenas os números ímpares](#questão-2).
 
3. [Crie um array de números (positivos e negativos). Você deve retornar a soma dos números positivos do mesmo](#questão-3).
 
4. [Crie uma string com alguns espaços vazios, depois remova os espaços e imprima no console a nova string](#questão-4).

5. [Faça um script que pede duas notas de um aluno. Em seguida ele deve calcular a média do aluno e dar o seguinte resultado:](#questão-5)

   + A mensagem "Aprovado", se a média alcançada for maior ou igual a sete;
   + A mensagem "Reprovado", se a média for menor do que sete;
   + A mensagem "Aprovado com Distinção", se a média for igual a dez.

6. [xxx](#questão-6)

7. [xxx](#questão-7)

8. [xxx](#questão-8)

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

### Questão 6
### Questão 7
### Questão 8
