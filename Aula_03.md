# Conceitos de Crud e comandos
<br>

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
