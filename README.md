```
#######################################
###                                 ###
###     Desenvolvido por Panda      ###
###                                 ###
#######################################
```


# API de Gerenciamento de Tarefas (.NET + PostgreSQL)

## OBJETIVO

Esta API tem como finalidade gerenciar tarefas, permitindo o cadastro, visualizacao, edicao e exclusao de tarefas em um banco de dados PostgreSQL.

## TECNOLOGIAS UTILIZADAS

- .NET 8
- C#
- PostgreSQL
- Entity Framework Core
- Swagger (Swashbuckle)

## FUNCIONALIDADES

- Criar tarefa
- Listar todas as tarefas
- Buscar tarefa por ID
- Buscar tarefas por palavra-chave 
- Atualizar tarefa
- Deletar tarefa

## MODELO DE DADOS

```csharp
public class Task
{
    public int ID { get; set; }
    public string Title { get; set; }
    public string Description { get; set; }
    public DateTime InitialDate { get; set; }
    public DateTime? ClosedDate { get; set; }
    public bool Completed { get; set; }
}