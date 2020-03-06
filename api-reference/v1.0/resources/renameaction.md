---
author: daspek
ms.author: dspektor
title: tipo de recurso renameaction
description: O objeto renameaction fornece informações sobre uma atividade que renomeia um item.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: b21d4630ca29aff9322d5114a5048b42f19fa4a0
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533845"
---
# <a name="renameaction-resource-type"></a>tipo de recurso renameaction

Namespace: microsoft.graph

A presença do recurso **renameaction** em uma [**myactivity**][activity] indica que a atividade renomeou um item.

>**Observação:** Os registros de atividade de item atualmente só estão disponíveis no SharePoint e no OneDrive for Business.

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
