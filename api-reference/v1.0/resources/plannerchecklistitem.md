---
title: Tipo de recurso plannerChecklistItem
description: O recurso de **plannerChecklistItem** representa um item na lista de verificação de uma tarefa. A lista de verificação em uma tarefa é representada pelo objeto itens.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 554391577fb0d48c2e0fd9fe265298e1dc1dd4fb
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27941664"
---
# <a name="plannerchecklistitem-resource-type"></a>Tipo de recurso plannerChecklistItem


O recurso **plannerChecklistItem** representa um item da lista de verificação de uma tarefa. A lista de verificação em uma tarefa é representada pelo [objeto checklistItems](plannerchecklistitems.md).


## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|isChecked|Booliano|O valor será `true` se o item estiver marcado ou `false`, caso não estiver marcado.|
|lastModifiedBy|[identitySet](identityset.md)| Somente leitura. A identificação de usuário pela qual isso foi modificado pela última vez.|
|lastModifiedDateTime|DateTimeOffset|Somente leitura. A data e a hora pelas quais isso foi modificado pela última vez. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|orderHint|String|Usado para definir a ordem relativa dos itens na lista de verificação. O formato é definido como descrito [aqui](planner-order-hint-format.md).|
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
<!-- {
  "type": "#page.annotation",
  "description": "plannerChecklistItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
