---
title: Tipo de recurso educationClass
description: Representa uma aula em uma escola. O **recurso educationClass** corresponde ao grupo Microsoft 365 e compartilha a mesma ID.
ms.localizationpriority: medium
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 50302c03f9ccd1bd1b1ea38717be539a0731941b
ms.sourcegitcommit: c21fefa5c3c62df14147e7918cb43327f7d72e69
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/06/2022
ms.locfileid: "64685092"
---
# <a name="educationclass-resource-type"></a>Tipo de recurso educationClass

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma aula em uma escola. O **recurso educationClass** atualmente corresponde a um grupo Microsoft 365 [e] compartilha a mesma ID.
Os alunos são membros regulares da classe e os professores são proprietários e têm direitos apropriados.

> [!IMPORTANT]
> Para Microsoft 365 experiências funcionem corretamente, os professores devem ser membros das coleções de professores e membros.

## <a name="methods"></a>Métodos

| Método                                                                  | Tipo de retorno                                    | Descrição                                                                               |
| :---------------------------------------------------------------------- | :--------------------------------------------- | :---------------------------------------------------------------------------------------- |
| [Obter educationClass](../api/educationclass-get.md)                      | [educationClass]                               | Leia as propriedades e relações de um objeto **educationClass**.                        |
| [Adicionar membro](../api/educationclass-post-members.md)                     | [educationUser]                                | Adicione um novo **educationUser** para a aula postando na propriedade de navegação de membros.  |
| [Listar membros](../api/educationclass-list-members.md)                   | Coleção [educationUser]                     | Obtenha uma coleção de objetos **educationUser**.                                               |
| [Remover alunos](../api/educationclass-delete-members.md)               | [educationUser]                                | Remova um **educationUser** da aula por meio da propriedade de navegação de membros.       |
| [Listar escolas](../api/educationclass-list-schools.md)                   | Coleção [educationSchool]                   | Obtenha uma coleção de objetos **educationSchool**.                                             |
| [Adicionar professor](../api/educationclass-post-teachers.md)                   | [educationUser]                                | Adicione um novo **educationUser** para a aula postando na propriedade de navegação de professores. |
| [Listar professores](../api/educationclass-list-teachers.md)                 | Coleção [educationUser]                     | Obtenha uma lista de professores para a aula.                                                     |
| [Remover professor](../api/educationclass-delete-teachers.md)              | [educationUser]                                | Remova um **educationUser** da aula por meio da propriedade de navegação de professores.      |
| [Criar educationAssignment](../api/educationclass-post-assignments.md) | [educationAssignment]                          | Crie um novo **educationAssignment** postando na coleção de tarefas.            |
| [Listar tarefas](../api/educationclass-list-assignments.md)           | [educationAssignmentcollection]                | Obtenha uma **coleção de objetos educationAssignment** .                                         |
| [Obter grupo](../api/educationclass-get-group.md)                         | [group]                                        | Obtenha o Microsoft 365 **grupo** que corresponde a esta **educationClass**.              |
| [Criar educationCategory](../api/educationclass-post-category.md)      | [educationCategory]                            | Crie uma **nova educationCategory** para esta classe.                                        |
| [Listar categorias](../api/educationclass-list-categories.md)             | [coleção educationCategory]                 | Obtenha uma lista de **objetos educationCategory** que pertencem a essa classe.                      |
| [Atualizar](../api/educationclass-update.md)                               | [educationClass]                               | Atualize o objeto **educationClass**.                                                         |
| [Delete](../api/educationclass-delete.md)                               | Nenhuma                                           | Exclua o objeto **educationClass**.                                                         |
| [Obter delta](../api/educationclass-delta.md)                                 | Coleção [educationClass](educationclass.md) | Obter alterações incrementais para **educationClasses**.                                          |

## <a name="properties"></a>Propriedades

| Propriedade             | Tipo                                  | Descrição                                                                                                                                                          |
| :------------------- | :------------------------------------ | :------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| id                   | Cadeia de caracteres                                | O identificador exclusivo da aula.                                                                                                                                     |
| classCode            | Cadeia de caracteres                                | Código de aula usada pela escola para identificar a aula.                                                                                                                 |
| Curso               | [educationCourse](educationcourse.md) | Informações do curso para a aula.                                                                                                                                     |
| createdBy            | [identitySet]                         | Entidade que criou a classe.                                                                                                                                         |
| description          | Cadeia de caracteres                                | Descrição da aula.                                                                                                                                            |
| displayName          | String                                | Nome da aula.                                                                                                                                                   |
| externalId           | Cadeia de caracteres                                | ID da aula no sistema de sincronização.                                                                                                                             |
| externalName         | Cadeia de caracteres                                | Nome da aula no sistema de sincronização.                                                                                                                             |
| externalSource       | String                                | O tipo de fonte externa da qual esse recurso foi gerado (determinado automaticamente de `externalSourceDetail`). Os valores possíveis são: `sis`, `lms` ou `manual`. |
| externalSourceDetail | Cadeia de caracteres                                | O nome da fonte externa da qual esses recursos foram gerados.                                                                                                   |
| grade                | Cadeia de caracteres                                | Nível de nota da classe.                                                                                                                                            |
| mailNickname         | String                                | Nome de email para enviar email a todos os membros, se essa propriedade estiver habilitada.                                                                                                      |
| term                 | [educationTerm]                       | Termo para a classe.                                                                                                                                                  |

## <a name="relationships"></a>Relações

| Relação | Tipo                             | Descrição                                               |
| :----------- | :------------------------------- | :-------------------------------------------------------- |
| assignments  | [coleção educationAssignment] | Todas as atribuições associadas a essa classe. Anulável.     |
| members      | Coleção [educationUser]       | Todos os usuários da aula. Anulável.                         |
| schools      | Coleção [educationSchool]     | Todas as escolas às quais essa aula está associada. Anulável. |
| teachers     | Coleção [educationUser]       | Todos os professores da aula. Anulável.                      |
|assignmentCategories| [coleção educationCategory](educationcategory.md) | Todas as categorias associadas a essa classe. Anulável. |
|assignmentDefaults| [coleção educationAssignmentDefaults](educationassignmentdefaults.md) | Especifica padrões de nível de classe respeitados por novas atribuições criadas na classe. |
|assignmentSettings| [coleção educationAssignmentSettings](educationassignmentsettings.md) | Especifica as configurações de atribuições de nível de classe. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationClass"
}-->

```json
{
  "classCode": "String",
  "course": { "@odata.type": "microsoft.graph.educationCourse" },
  "createdBy": { "@odata.type": "microsoft.graph.identitySet" },
  "description": "String",
  "displayName": "String",
  "externalId": "String",
  "externalName": "String",
  "externalSource": "string",
  "grade": "string",
  "id": "String (identifier)",
  "mailNickname": "String",
  "term": { "@odata.type": "microsoft.graph.educationTerm" }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.educationClass",
  "description": "educationUser resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]

}-->

[educationclass]: educationclass.md
[educationuser]: educationuser.md
[educationassignment]: educationassignment.md
[educationcourse]: educationcourse.md
[educationcategory]: educationcategory.md
[educationschool]: educationschool.md
[educationterm]: educationterm.md
[identityset]: identityset.md
[group]: group.md


