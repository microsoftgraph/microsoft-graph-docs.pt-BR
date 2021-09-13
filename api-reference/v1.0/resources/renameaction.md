---
author: daspek
title: Tipo de recurso renameAction
description: O objeto renameAction fornece informações sobre uma atividade que renomeou um item.
ms.localizationpriority: medium
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: d513ae68a2f438483930dd51c40fa06bed626d5b
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59084157"
---
# <a name="renameaction-resource-type"></a>Tipo de recurso renameAction

Namespace: microsoft.graph

A presença do recurso **renameAction** em um [**itemActivity**][activity] indica que a atividade renomeou um item.

>**Observação:** No momento, os registros de atividade do item estão disponíveis apenas SharePoint e OneDrive for Business.

[activity]: itemactivity.md

## <a name="properties"></a>Propriedades

| Nome da propriedade | Tipo   | Descrição
|:--------------|:-------|:----------------------------------------------------
| oldName       | string | O nome anterior do item.
| newName       | cadeia de caracteres | O novo nome do item.

## <a name="json-representation"></a>Representação JSON

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type&quot;: &quot;microsoft.graph.renameAction"
}-->

```json
{
  "oldName": "string",
  "newName&quot;: &quot;string"
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

