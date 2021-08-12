---
author: daspek
title: Tipo de recurso moveAction
description: O objeto MoveAction fornece informações sobre uma atividade que moveu um item.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 160afbc51196c60473dc40bec7b79daab6dc39eb3f302c1a1b9689c9c25929fe
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54189461"
---
# <a name="moveaction-resource-type"></a>Tipo de recurso moveAction

Namespace: microsoft.graph

A presença do recurso **moveAction** em um [**itemActivity**][activity] indica que a atividade moveu um item.

>**Observação:** No momento, os registros de atividade do item estão disponíveis apenas SharePoint e OneDrive for Business.

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
  "@type&quot;: &quot;microsoft.graph.moveAction"
}-->

```json
{
  "from": "string",
  "to&quot;: &quot;string"
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

