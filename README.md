📘 Métodos de Array no JavaScript: map, filter e reduce

👥 Lista de Convidados (Exemplo Base)

```const convidadados = [
    {nome: "Fernando", idade: 20 , cidade: "João Pessoa"},
    { nome: "José", idade: 15, cidade: "Duas Estradas" },
    { nome: "Ana", idade: 23, cidade: "João Pessoa" },
    { nome: "Bernado", idade: 18, cidade: "Bananeiras" },
    { nome: "Luana", idade: 25, cidade: "Cabedelo" }
]
```

🔄 map()

Usamos o map quando se torna necessário percorrer o array e alterar os elementos.
O map irá criar uma cópia da lista onde será possível manipular os elementos e objetos e adicionar novas propriedades a eles.

✔ Exemplo
```
let indiceConvidados = convidadados.map((convidado,index) => {
    return { ...convidado, index}
})
```
🔍 filter()

Usamos o filter para filtrar os dados.
Ou seja, selecionar apenas alguns elementos/objetos do array que estejam de acordo com a condição estabelecida para a filtragem.

✔ Exemplo
```
let maioresDeIdade = convidadados.filter((convidado) => {
    return convidado.idade >= 18
})
```
🧮 reduce()

O reduce serve quando você quer gerar um único resultado a partir de todos os elementos do array, que pode ser um número, objeto, string ou outra estrutura.

✔ Exemplo
```
let somaIdades = convidadados.reduce((total, convidado) => {
    return total + convidado.idade
}, 0)
```
