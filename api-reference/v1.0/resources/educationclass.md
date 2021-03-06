---
title: Tipo de recurso educationClass
description: 'Representa uma aula em uma escola. O recurso **educationClass** corresponde ao grupo Microsoft 365 e compartilha a mesma ID. Os alunos são membros regulares da aula e os professores são proprietários e têm direitos apropriados. Para que as experiências do Office funcionem corretamente, os professores devem ser membros das coleções de professores e membros.  '
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 57e3204e15755e9ec7ce0150f46c6f0409ca3120
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48032688"
---
# <a name="educationclass-resource-type"></a>Tipo de recurso educationClass

Namespace: microsoft.graph

Representa uma aula em uma escola. O recurso **educationClass** corresponde ao grupo Microsoft 365 e compartilha a mesma ID. Os alunos são membros regulares da aula e os professores são proprietários e têm direitos apropriados. Para que as experiências do Office funcionem corretamente, os professores devem ser membros das coleções de professores e membros.  


## <a name="methods"></a>Methods

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
|[Obter grupo](../api/educationclass-get-group.md) |[group](group.md)| Obtenha o **grupo** Microsoft 365 que corresponde a esse **educationClass**.|
|[Atualizar](../api/educationclass-update.md) | [educationClass](educationclass.md)    |Atualize o objeto **educationClass**. |
|[Delete](../api/educationclass-delete.md) | Nenhum |Exclua o objeto **educationClass**. |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|id| String| O identificador exclusivo da aula.|
|description|String| Descrição da aula.|
|displayName|String| Nome da aula.|
|mailNickname|String| Nome de email para enviar email a todos os membros, se essa propriedade estiver habilitada. |
|createdBy|[identitySet](identityset.md)| Entidade que criou a aula |
|classCode|Cadeia de caracteres| Código de aula usada pela escola para identificar a aula.|
|externalId|Cadeia de caracteres| ID da aula no sistema de sincronização. |
|externalName|Cadeia de caracteres|Nome da aula no sistema de sincronização.|
|externalSource|educationExternalSource| Como essa aula foi criada. Os valores possíveis são: `sis`, `manual`, `unknownFutureValue`.|
|term|[educationTerm](educationterm.md)|Termos dessa aula.|

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|membros|Coleção [educationUser](../resources/educationuser.md)| Todos os usuários da aula. Anulável.|
|schools|Coleção [educationSchool](../resources/educationschool.md)| Todas as escolas às quais essa aula está associada. Anulável.|
|teachers|Coleção [educationUser](../resources/educationuser.md)|  Todos os professores da aula. Anulável.|
|group|[group](../resources/group.md)| O grupo de diretórios correspondente a esta classe.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
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
<!-- {
  "type": "#page.annotation",
  "description": "educationClass resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

