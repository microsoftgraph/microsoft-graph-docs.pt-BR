---
title: Tipo de recurso plannerChecklistItem
description: O **recurso plannerChecklistItem** representa um item na lista de verificação de uma tarefa. A lista de verificação em uma tarefa é representada pelo objeto checklistItems.
ms.localizationpriority: medium
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: a8ba68b0b9e9bb3bf6979ad9eb3d498fe55b80ee
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59113543"
---
# <a name="plannerchecklistitem-resource-type"></a>Tipo de recurso plannerChecklistItem

Namespace: microsoft.graph


O **recurso plannerChecklistItem** representa um item na lista de verificação de uma tarefa. A lista de verificação em uma tarefa é representada pelo [objeto checklistItems](plannerchecklistitems.md).


## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|isChecked|Boolean|O valor `true` é se o item for verificado e caso `false` contrário.|
|lastModifiedBy|[identitySet](identityset.md)| Somente leitura. ID do usuário pela qual foi modificada pela última vez.|
|lastModifiedDateTime|DateTimeOffset|Somente leitura. Data e hora em que isso foi modificado pela última vez. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`|
|orderHint|String|Usado para definir a ordem relativa de itens na lista de verificação. O formato é definido como descrito [aqui](planner-order-hint-format.md).|
|title|Cadeia de caracteres|Título do item de lista de verificação|

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

