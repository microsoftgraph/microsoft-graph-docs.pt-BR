---
author: daspek
description: A presença do recurso DeleteAction em uma itemActivity indica que a atividade excluiu um item.
ms.date: 09/14/2017
title: DeleteAction
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 453be9ad3764081207cfa51e56b69111186ff87b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507272"
---
# <a name="deleteaction-resource-type"></a>Tipo de recurso DeleteAction

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

A presença do recurso **DeleteAction** em uma [**itemActivity**][activity] indica que a atividade excluiu um item.

[activity]: itemactivity.md

## <a name="json-representation"></a>Representação JSON

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.deleteAction"
}-->

```json
{
  "name": "string",
  "objectType": "File | Folder"
}
```

## <a name="properties"></a>Propriedades

| Nome da propriedade | Tipo   | Descrição
|:--------------|:-------|:----------------------------------------------------
| nome          | string | O nome do item que foi excluído.
| objectType    | string | `File`ou `Folder`, dependendo do tipo do item excluído.

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
