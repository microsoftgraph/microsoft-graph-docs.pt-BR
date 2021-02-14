---
author: daspek
title: Tipo de recurso deleteAction
description: O objeto deleteAction fornece informações sobre a exclusão de um item.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: e78b4369606b0e0e3880fc3bfd13fdec263fcb58
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/14/2021
ms.locfileid: "50239629"
---
# <a name="deleteaction-resource-type"></a>Tipo de recurso deleteAction

Namespace: microsoft.graph

A presença do recurso **deleteAction** em um [**itemActivity**][activity] indica que a atividade excluiu um item.

>**Observação:** No momento, os registros de atividades do item só estão disponíveis no SharePoint e no OneDrive for Business.

[activity]: itemactivity.md

## <a name="properties"></a>Propriedades

| Nome da propriedade | Tipo   | Descrição
|:--------------|:-------|:----------------------------------------------------
| name          | string | O nome do item que foi excluído.
| objectType    | string | `File` ou `Folder` , dependendo do tipo do item excluído.


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

