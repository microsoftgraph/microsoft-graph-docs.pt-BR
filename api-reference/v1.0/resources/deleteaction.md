---
author: daspek
ms.author: dspektor
title: tipo de recurso DeleteAction
description: O objeto DeleteAction fornece informações sobre a exclusão de um item.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 0bd96e02e822d1b2e1901667cbbea86ca91c8b3e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48018729"
---
# <a name="deleteaction-resource-type"></a>tipo de recurso DeleteAction

Namespace: microsoft.graph

A presença do recurso **DeleteAction** em uma [**myactivity**][activity] indica que a atividade excluiu um item.

>**Observação:** Os registros de atividade de item atualmente só estão disponíveis no SharePoint e no OneDrive for Business.

[activity]: itemactivity.md

## <a name="properties"></a>Propriedades

| Nome da propriedade | Tipo   | Descrição
|:--------------|:-------|:----------------------------------------------------
| nome          | string | O nome do item que foi excluído.
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

