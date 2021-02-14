---
author: daspek
title: Tipo de recurso renameAction
description: O objeto renameAction fornece informações sobre uma atividade que renomeou um item.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 35e0aa9929b8e152265a5540625f5981a587edb7
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/14/2021
ms.locfileid: "50238649"
---
# <a name="renameaction-resource-type"></a>Tipo de recurso renameAction

Namespace: microsoft.graph

A presença do recurso **renameAction** em um [**itemActivity**][activity] indica que a atividade renomeou um item.

>**Observação:** No momento, os registros de atividades do item só estão disponíveis no SharePoint e no OneDrive for Business.

[activity]: itemactivity.md

## <a name="properties"></a>Propriedades

| Nome da propriedade | Tipo   | Descrição
|:--------------|:-------|:----------------------------------------------------
| oldName       | string | O nome anterior do item.
| newName       | string | O novo nome do item.

## <a name="json-representation"></a>Representação JSON

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.renameAction"
}-->

```json
{
  "oldName": "string",
  "newName": "string"
}
```

<!--
{
  "type": "#page.annotation",
  "description": "The renameAction object provides information about an activity that renamed an item.",
  "keywords": "activities,activity,action,rename,renamed",
  "section": "documentation",
  "tocPath": "Resources/renameAction",
  "suppressions": []
}
-->

