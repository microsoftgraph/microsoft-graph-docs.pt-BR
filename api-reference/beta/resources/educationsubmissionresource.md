---
title: tipo de recurso educationSubmissionResource
description: 'Um wrapper em torno de um recurso para uso em um envio. O wrapper adiciona um ponteiro ao recurso de atribuição se ele foi copiado da atribuição.  '
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 48f4549354603346e39b5e1f6f387b207e2f14ef
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972478"
---
# <a name="educationsubmissionresource-resource-type"></a>tipo de recurso educationSubmissionResource

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um wrapper em torno de um recurso para uso em um envio. O wrapper adiciona um ponteiro ao recurso de atribuição se ele foi copiado da atribuição.  


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Obter educationSubmissionResource](../api/educationsubmissionresource-get.md) | [educationSubmissionResource](educationsubmissionresource.md) |Ler propriedades e relações de um objeto **educationSubmissionResource** .|
|[Delete](../api/educationsubmissionresource-delete.md) | None |Excluir um objeto **educationSubmissionResource** . |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|assignmentResourceUrl|String|Ponteiro para a atribuição da qual este recurso foi copiado. Se isso for nulo, o aluno carregou o recurso.|
|id|String| Somente leitura.|
|recurso|[educationResource](educationresource.md)|Objeto Resource.|

## <a name="relationships"></a>Relações
Nenhum


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationSubmissionResource"
}-->

```json
{
  "assignmentResourceUrl": "String",
  "id": "String (identifier)",
  "resource": {"@odata.type": "microsoft.graph.educationResource"}
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationSubmissionResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
