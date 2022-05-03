---
author: daspek
description: A presença do recurso MoveAction em uma itemActivity indica que a atividade moveu um item.
ms.date: 09/14/2017
title: MoveAction
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: sites-and-lists
ms.openlocfilehash: f3622067f273a587174494d2ce3a68ed56540883
ms.sourcegitcommit: 267e3baf545c8dc71ba2ab69497e3ec369379f43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/03/2022
ms.locfileid: "65176549"
---
# <a name="moveaction-resource-type"></a>Tipo de recurso MoveAction

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

A presença do recurso **MoveAction** em uma [**itemActivity**][activity] indica que a atividade moveu um item.

[activity]: itemactivity.md

## <a name="json-representation"></a>Representação JSON

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type&quot;: &quot;microsoft.graph.moveAction"
}-->

```json
{
  "from": "string",
  "to&quot;: &quot;string"
}
```

## <a name="properties"></a>Propriedades

| Propriedade | Tipo   | Descrição                                       |
| :------- | :----- | :------------------------------------------------ |
| from     | string | O nome do local do qual o item foi movido. |
| para       | string | O nome do local para o qual o item foi movido.   |

## <a name="remarks"></a>Comentários

Registros de atividade de item atualmente só estão disponíveis no SharePoint e no OneDrive for Business.

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
