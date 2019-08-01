---
author: daspek
ms.author: dspektor
title: tipo de recurso renameaction
description: O objeto renameaction fornece informações sobre uma atividade que renomeia um item.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 2949a3875d657dba3c64b6753855476c1d66bfb3
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36034717"
---
# <a name="renameaction-resource-type"></a>tipo de recurso renameaction

A presença do recurso **** renameaction em uma myactivity indica que a atividade renomeou um item. [****][activity]

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
