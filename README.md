Usamos o Map quando se torna necessario pecorrer o array e alerar os elementos. O map irá criar uma cópia da lista onde será posível manipular os elementos e objetos e adicionar novas propriedades a eles
Exemplo:

const convidadados = [
    {nome: "Fernando", idade: 20 , cidade: "João Pessoa"},
    { nome: "José", idade: 15, cidade: "Duas Estradas" },
    { nome: "Ana", idade: 23, cidade: "João Pessoa" },
    { nome: "Bernado", idade: 18, cidade: "Bananeiras" },
    { nome: "Luana", idade: 25, cidade: "Cabedelo" }
]

let indiceConvidados = convidadados.map((convidado,index) => {
    return { ...convidado, index}
})


