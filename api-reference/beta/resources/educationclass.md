---
title: Tipo de recurso educationClass
description: Representa uma aula em uma escola. O recurso **educationClass** corresponde ao grupo do Office 365 e compartilha a mesma ID.
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: d3a7f4e49f50ca4cb26e52d767064cc57b255ce4
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/27/2019
ms.locfileid: "36633703"
---
# <a name="educationclass-resource-type"></a>Tipo de recurso educationClass

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma aula em uma escola. O recurso **educationClass** corresponde ao grupo do Office 365 e compartilha a mesma ID. Os alunos são membros regulares da aula e os professores são proprietários e têm direitos apropriados. Para que as experiências do Office 365 funcionem corretamente, os professores devem ser membros das coleções de professores e membros.

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
| [Criar educationAssignment](../api/educationclass-post-assignments.md) | [educationAssignment]                          | Crie um novo **educationAssignment** postando na coleção assignments.            |
| [Listar tarefas](../api/educationclass-list-assignments.md)           | coleção [educationAssignment]                | Obtenha uma coleção de objetos **educationAssignment** .                                         |
| [Obter grupo](../api/educationclass-get-group.md)                         | [group]                                        | Recupere o **group** do Office 365 que corresponde a essa **educationClass**.                 |
| [Criar educationCategory](../api/educationclass-post-category.md)      | [educationCategory]                            | Crie um novo **educationCategory** para esta classe.                                        |
| [Listar categorias](../api/educationclass-list-categories.md)             | coleção [educationCategory]                 | Obtenha uma lista de objetos **educationCategory** pertencentes a essa classe.                      |
| [Atualizar](../api/educationclass-update.md)                               | [educationClass]                               | Atualize o objeto **educationClass**.                                                         |
| [Delete](../api/educationclass-delete.md)                               | Nenhum                                           | Exclua o objeto **educationClass**.                                                         |
| [Delta](../api/educationclass-delta.md)                                 | Coleção [educationClass](educationclass.md) | Obter alterações incrementais para o **educationClasses**                                          |

## <a name="properties"></a>Propriedades

| Propriedade       | Tipo                                  | Descrição                                                                             |
| :------------- | :------------------------------------ | :-------------------------------------------------------------------------------------- |
| id             | Cadeia de caracteres                                | O identificador exclusivo da aula.                                                        |
| classCode      | String                                | Código de aula usada pela escola para identificar a aula.                                    |
| durante         | [educationCourse](educationcourse.md) | Informações de cursos da turma                                                        |
| createdBy      | [identitySet]                         | Entidade que criou a aula                                                            |
| descrição    | String                                | Descrição da aula.                                                               |
| displayName    | String                                | Nome da aula.                                                                      |
| externalId     | String                                | ID da aula no sistema de sincronização.                                                |
| externalName   | Cadeia de caracteres                                | Nome da aula no sistema de sincronização.                                                |
| externalSource | cadeia de caracteres                                | Como essa aula foi criada. Os valores possíveis são: `sis`, `manual`, `unknownFutureValue`. |
| grade          | string                                | Nível de graduação da turma.                                                               |
| mailNickname   | String                                | Nome de email para enviar email a todos os membros, se essa propriedade estiver habilitada.                         |
| term           | [educationTerm]                       | Termo para a classe.                                                                     |

## <a name="relationships"></a>Relações

| Relação | Tipo                             | Descrição                                               |
| :----------- | :------------------------------- | :-------------------------------------------------------- |
| assignments  | coleção [educationAssignment] | Todas as atribuições associadas a esta classe. Anulável.     |
| members      | Coleção [educationUser]       | Todos os usuários da aula. Anulável.                         |
| schools      | Coleção [educationSchool]     | Todas as escolas às quais essa aula está associada. Anulável. |
| teachers     | Coleção [educationUser]       | Todos os professores da aula. Anulável.                      |

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
    "Error: Resource educationClass has documented navigation properties, but we thought it was a complex type!",
    "Resource educationClass has documented navigation properties, but we thought it was a complex type!"
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
