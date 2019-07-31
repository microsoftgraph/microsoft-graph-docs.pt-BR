---
title: tipo de recurso plannerChecklistItem
description: O recurso **plannerChecklistItem** representa um item na lista de verificação de uma tarefa. A lista de verificação em uma tarefa é representada pelo objeto checklistItems.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 9bce6b0089f9e713e66e0354ce58d68cfd17fa7c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009073"
---
# <a name="plannerchecklistitem-resource-type"></a>tipo de recurso plannerChecklistItem

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O recurso **plannerChecklistItem** representa um item na lista de verificação de uma tarefa. A lista de verificação em uma tarefa é representada pelo [objeto checklistItems](plannerchecklistitems.md).


## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|IsChecked|Booliano|Value é `true` se o item estiver marcado e `false` , caso contrário.|
|lastModifiedBy|[identitySet](identityset.md)| Somente leitura. ID de usuário pela qual esta foi modificada pela última vez.|
|lastModifiedDateTime|DateTimeOffset|Somente leitura. Data e hora da última modificação. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|orderHint|String|Usado para definir a ordem relativa dos itens na lista de verificação. O formato é definido conforme descrito [aqui](planner-order-hint-format.md).|
|title|String|Título do item de lista de verificação|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerChecklistItem"
}-->

```json
{
  "isChecked": true,
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "String (timestamp)",
  "orderHint": "String",
  "title": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "plannerChecklistItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
