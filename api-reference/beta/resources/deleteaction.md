---
author: daspek
description: A presença do recurso DeleteAction em uma itemActivity indica que a atividade excluiu um item.
ms.date: 09/14/2017
title: DeleteAction
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: sites-and-lists
ms.openlocfilehash: e7fcdac76d208bcb2f2fe79ca51d95ac89ef23ae
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/08/2022
ms.locfileid: "65944875"
---
# <a name="deleteaction-resource-type"></a>Tipo de recurso DeleteAction

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

A presença do recurso **DeleteAction** em uma [**itemActivity**][activity] indica que a atividade excluiu um item.

[activity]: itemactivity.md

## <a name="json-representation"></a>Representação JSON

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type&quot;: &quot;microsoft.graph.deleteAction"
}-->

```json
{
  "name": "string",
  "objectType&quot;: &quot;File | Folder"
}
```

## <a name="properties"></a>Propriedades

| Propriedade   | Tipo   | Descrição                                                    |
| :--------- | :----- | :------------------------------------------------------------- |
| nome       | string | O nome do item que foi excluído.                         |
| objectType | cadeia de caracteres | `File` ou `Folder`, dependendo do tipo do item excluído. |

## <a name="remarks"></a>Comentários

Registros de atividade de item atualmente só estão disponíveis no SharePoint e no OneDrive for Business.

<!--
{
  "type": "#page.annotation",
  "description": "The DeleteAction object provides information about the deletion of an item.",
  "keywords": "activities,activity,action,delete,deletion",
  "section": "documentation",
  "tocPath": "Resources/DeleteAction",
  "suppressions": []
}
-->
