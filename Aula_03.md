# Conceitos de Crud e comandos

[<- VOLTAR](https://github.com/igorcardiias?tab=repositories)

CRUD são as quatro operações fundamentais em qualquer banco de dados:

🟢 C → Create (criar): Inserir novos documentos em uma coleção

🔵 R → Read (ler/consultar): Consultar dados armazenados

🟠 U → Update (atualizar): Alterar informações de documentos existentes

🔴 D → Delete (excluir): Remover documentos do banco

## ------------------------------------------------

## Primeira inserção no MongoDB de um documento

### Código: db["aula_crud"].insertOne({})

    db["aula_crud"].insertOne({
        nome: "Zé da Manga",
        idade: 23,
        curso: "Engenharia",
        notas: [8.5, 9.0, 7.0],
        ativo: true
})

## Inserir VÁRIOS documentos de uma vez

### Código: db["aula_crud"].insertMany([])

    db["aula_crud"].insertMany([
      {
        nome: "Bruno",
        idade: 21,
        curso: "Medicina",
        notas: [9.5, 8.0],
        ativo: true
      },

      {
        nome: "Carla",
        idade: 25,
        curso: "Direito",
        notas: [7.0, 6.5, 8.0],
        ativo: false
      },

      {
        nome: "Diego",
        idade: 22,
        curso: "Computação",
        notas: [8.0, 9.0],
        ativo: true
    }
    ])

## Para fazer buscas em um campo específico no MongoDB

### Código: db["aula_crud"].find().pretty()

      db["aula_crud"].find({ nome: "Zé da Manga" }).pretty()
### ----------------------------------------------------------      

## Buscar com projeção (mostrar apenas nome e curso, sem _id)

    db["aula_crud"].find(
    { ativo: true },
    { nome: 1, curso: 1, _id: 0 }
    )     


## 🔑 Operadores de consulta(Buscas):

    
    $gt: maior que
    
    $lt: menor que
    
    $gte: maior ou igual
    
    $lte: menor ou igual
    
    $ne: diferente
    
    $in: está na lista

## ------------------------------------------------
## 🔑 Operadores de atualização:
    
    $set: define valor (cria se não existe)
    
    $inc: incrementa valor numérico
    
    $push: adiciona item ao array
    
    $pull: remove item do array
    
    $unset: remove campo






   [<- VOLTAR](https://github.com/igorcardiias/Banco-de-Dados-N-o-Relacionais.git)  

