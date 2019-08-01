---
author: daspek
ms.author: dspektor
title: tipo de recurso DeleteAction
description: O objeto DeleteAction fornece informações sobre a exclusão de um item.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 93f605e74a0a483a94593a9aaa40d6fd30efe914
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36032729"
---
# <a name="deleteaction-resource-type"></a>tipo de recurso DeleteAction

A presença do recurso **DeleteAction** em uma myactivity indica que a atividade excluiu um item. [****][activity]

>**Observação:** Os registros de atividade de item atualmente só estão disponíveis no SharePoint e no OneDrive for Business.

[activity]: itemactivity.md

## <a name="properties"></a>Propriedades

| Nome da propriedade | Tipo   | Descrição
|:--------------|:-------|:----------------------------------------------------
| name          | string | O nome do item que foi excluído.
| objectType    | string | `File`ou `Folder`, dependendo do tipo do item excluído.


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

<!--
{
  "type": "#page.annotation",
  "description": "The deleteAction object provides information about the deletion of an item.",
  "keywords": "activities,activity,action,delete,deletion",
  "section": "documentation",
  "tocPath": "Resources/DeleteAction",
  "suppressions": []
}
-->
