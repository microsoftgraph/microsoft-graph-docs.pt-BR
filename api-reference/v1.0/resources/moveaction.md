---
author: daspek
title: Tipo de recurso moveAction
description: O objeto MoveAction fornece informações sobre uma atividade que moveu um item.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 2f588ecabefa1425f47d3efec6728587fb694798
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/14/2021
ms.locfileid: "50239335"
---
# <a name="moveaction-resource-type"></a>Tipo de recurso moveAction

Namespace: microsoft.graph

A presença do recurso **moveAction** em um [**itemActivity**][activity] indica que a atividade moveu um item.

>**Observação:** No momento, os registros de atividades do item só estão disponíveis no SharePoint e no OneDrive for Business.

[activity]: itemactivity.md

## <a name="properties"></a>Propriedades

| Nome da propriedade | Tipo   | Descrição
|:--------------|:-------|:----------------------------------------------------
| from          | string | O nome do local do qual o item foi movido.
| para            | string | O nome do local para o qual o item foi movido.

## <a name="json-representation"></a>Representação JSON

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.moveAction"
}-->

```json
{
  "from": "string",
  "to": "string"
}
```

<!--
{
  "type": "#page.annotation",
  "description": "The MoveAction object provides information about an activity that moved an item.",
  "keywords": "activities,activity,action,move,moved",
  "section": "documentation",
  "tocPath": "Resources/MoveAction",
  "suppressions": []
}
-->

