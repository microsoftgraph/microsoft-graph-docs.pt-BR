---
author: daspek
ms.author: dspektor
title: tipo de recurso MoveAction
description: O objeto MoveAction fornece informações sobre uma atividade que moveu um item.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: ec1ac8ccaae502f66e205571e17eb5ad3eced8e7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48020528"
---
# <a name="moveaction-resource-type"></a>tipo de recurso MoveAction

Namespace: microsoft.graph

A presença do recurso **MoveAction** em uma [**myactivity**][activity] indica que a atividade moveu um item.

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

