---
author: daspek
ms.author: dspektor
title: tipo de recurso MoveAction
description: O objeto MoveAction fornece informações sobre uma atividade que moveu um item.
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 525558d040109e637e2f3532d16c308a197e45fb
ms.sourcegitcommit: 52baf24d1d08096214b12f60e7c755291fe03ab5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2019
ms.locfileid: "33970617"
---
# <a name="moveaction-resource-type"></a>tipo de recurso MoveAction

A presença do recurso **MoveAction** em uma myactivity [****] [ activity] indica que a atividade moveu um item.

>**Observação:** Os registros de atividade de item atualmente só estão disponíveis no SharePoint e no OneDrive for Business.

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
