---
title: Tipo de recurso educationClass
description: 'Representa uma aula em uma escola. O recurso **educationClass** corresponde ao grupo do Office 365 e compartilha a mesma ID. Os alunos são membros regulares da aula e os professores são proprietários e têm direitos apropriados. Para que as experiências do Office funcionem corretamente, os professores devem ser membros das coleções de professores e membros.  '
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 2a1fb4434933a4cc41c9a84c54864f2211f40962
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33334421"
---
# <a name="educationclass-resource-type"></a>Tipo de recurso educationClass

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma aula em uma escola. O recurso **educationClass** corresponde ao grupo do Office 365 e compartilha a mesma ID. Os alunos são membros regulares da aula e os professores são proprietários e têm direitos apropriados. Para que as experiências do Office funcionem corretamente, os professores devem ser membros das coleções de professores e membros.  


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Obter educationClass](../api/educationclass-get.md) | [educationClass](educationclass.md) |Leia as propriedades e relações de um objeto **educationClass**.|
|[Adicionar membro](../api/educationclass-post-members.md) |[educationUser](educationuser.md)| Adicione um novo **educationUser** para a aula postando na propriedade de navegação de membros.|
|[Listar membros](../api/educationclass-list-members.md) |Coleção [educationUser](educationuser.md)| Obtenha uma coleção de objetos **educationUser**.|
|[Remover alunos](../api/educationclass-delete-members.md) |[educationUser](educationuser.md)| Remova um **educationUser** da aula por meio da propriedade de navegação de membros.|
|[Listar escolas](../api/educationclass-list-schools.md) |Coleção [educationSchool](educationschool.md)| Obtenha uma coleção de objetos **educationSchool**.|
|[Adicionar professor](../api/educationclass-post-teachers.md) |[educationUser](educationuser.md)| Adicione um novo **educationUser** para a aula postando na propriedade de navegação de professores.|
|[Listar professores](../api/educationclass-list-teachers.md) |Coleção [educationUser](educationuser.md)| Obtenha uma lista de professores para a aula.|
|[Remover professor](../api/educationclass-delete-teachers.md) |[educationUser](educationuser.md)| Remova um **educationUser** da aula por meio da propriedade de navegação de professores.|
|[Criar educationAssignment](../api/educationclass-post-assignments.md) |[educationAssignment](../resources/educationassignment.md)| Crie um novo **educationAssignment** postando na coleção assignments.|
|[Listar tarefas](../api/educationclass-list-assignments.md) |coleção [educationAssignment](../resources/educationassignment.md)| Obtenha uma coleção de objetos **educationAssignment** .|
|[Obter grupo](../api/educationclass-get-group.md) |[group](group.md)| Recupere o **group** do Office 365 que corresponde a essa **educationClass**.|
|[Criar educationCategory](../api/educationclass-post-category.md) | [educationCategory](educationCategory.md) | Crie um novo **educationCategory** para esta classe.|
|[Listar categorias](../api/educationclass-list-categories.md) | coleção [educationCategory](educationCategory.md) | Obtenha uma lista de objetos **educationCategory** pertencentes a essa classe.|
|[Atualizar](../api/educationclass-update.md) | [educationClass](educationclass.md)    |Atualize o objeto **educationClass**. |
|[Delete](../api/educationclass-delete.md) | Nenhum |Exclua o objeto **educationClass**. |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|id| Cadeia de caracteres| O identificador exclusivo da aula.|
|description|String| Descrição da aula.|
|displayName|String| Nome da aula.|
|mailNickname|String| Nome de email para enviar email a todos os membros, se essa propriedade estiver habilitada. |
|createdBy|[identitySet](identityset.md)| Entidade que criou a aula |
|classCode|String| Código de aula usada pela escola para identificar a aula.|
|externalId|String| ID da aula no sistema de sincronização. |
|externalName|Cadeia de caracteres|Nome da aula no sistema de sincronização.|
|externalSource|cadeia de caracteres| Como essa aula foi criada. Os valores possíveis são: `sis`, `manual`, `unknownFutureValue`.|
|term|[educationTerm](educationterm.md)|Termos dessa aula.|


## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|members|Coleção [educationUser](../resources/educationuser.md)| Todos os usuários da aula. Anulável.|
|schools|Coleção [educationSchool](../resources/educationschool.md)| Todas as escolas às quais essa aula está associada. Anulável.|
|teachers|Coleção [educationUser](../resources/educationuser.md)|  Todos os professores da aula. Anulável.|
|assignments|coleção [educationAssignment](../resources/educationassignment.md)| Todas as atribuições associadas a esta classe. Anulável.|
|categories|coleção [educationCategory](../resources/educationassignment.md)| Todas as categorias associadas a essa classe. Anulável.|

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
  "id": "String",
  "description": "String",
  "classCode": "String",
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "displayName": "String",
  "externalId": "String",
  "externalName": "String",
  "externalSource": "string",
  "mailNickname": "String",
  "term": {"@odata.type": "microsoft.graph.educationTerm"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationClass resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
