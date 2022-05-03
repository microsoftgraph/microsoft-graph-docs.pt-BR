---
author: daspek
description: A presença do recurso RenameAction em uma itemActivity indica que a atividade renomeou um item.
ms.date: 09/14/2017
title: RenameAction
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: files
ms.openlocfilehash: 01ffdffff58b6e7d3592cfa6493d17c3d8649efc
ms.sourcegitcommit: 267e3baf545c8dc71ba2ab69497e3ec369379f43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/03/2022
ms.locfileid: "65176865"
---
# <a name="renameaction-resource-type"></a>Tipo de recurso RenameAction

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

A presença do recurso **RenameAction** em uma [**itemActivity**][activity] indica que a atividade renomeou um item.

[activity]: itemactivity.md

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

## <a name="properties"></a>Propriedades

| Propriedade | Tipo   | Descrição                    |
| :------- | :----- | :----------------------------- |
| oldName  | string | O nome anterior do item. |
| Newname  | cadeia de caracteres | O novo nome do item.      |

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
