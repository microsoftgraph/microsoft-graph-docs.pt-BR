---
author: daspek
description: A presença do recurso RenameAction em uma itemActivity indica que a atividade renomeou um item.
ms.date: 09/14/2017
title: RenameAction
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 6745f932c0a2d9b92273f45e147439cfbd2ed911
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521128"
---
# <a name="renameaction-resource-type"></a>Tipo de recurso RenameAction

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

A presença do recurso **RenameAction** em uma [**itemActivity**][activity] indica que a atividade renomeou um item.

[activity]: itemactivity.md

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

## <a name="properties"></a>Propriedades

| Nome da propriedade | Tipo   | Descrição
|:--------------|:-------|:----------------------------------------------------
| oldName       | string | O nome anterior do item.
| newName       | string | O novo nome do item.

## <a name="remarks"></a>Comentários

Registros de atividade de item atualmente só estão disponíveis no SharePoint e no OneDrive for Business.

<!--
{
  "type": "#page.annotation",
  "description": "The RenameAction object provides information about an activity that renamed an item.",
  "keywords": "activities,activity,action,rename,renamed",
  "section": "documentation",
  "tocPath": "Resources/RenameAction",
  "suppressions": []
}
-->
