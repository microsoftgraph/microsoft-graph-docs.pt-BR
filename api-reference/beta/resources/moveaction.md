---
author: daspek
description: A presença do recurso MoveAction em uma itemActivity indica que a atividade moveu um item.
ms.date: 09/14/2017
title: MoveAction
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 9fbb19097b6a1401bd3c0b6dba4ce1fd5649e706
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009640"
---
# <a name="moveaction-resource-type"></a>Tipo de recurso MoveAction

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

A presença do recurso **MoveAction** em uma [**itemActivity**][activity] indica que a atividade moveu um item.

[activity]: itemactivity.md

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

## <a name="properties"></a>Propriedades

| Nome da propriedade | Tipo   | Descrição
|:--------------|:-------|:----------------------------------------------------
| from          | string | O nome do local do qual o item foi movido.
| para            | string | O nome do local para o qual o item foi movido.

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
