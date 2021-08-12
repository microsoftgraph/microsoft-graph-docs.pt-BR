---
author: daspek
title: Tipo de recurso deleteAction
description: O objeto deleteAction fornece informações sobre a exclusão de um item.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: c57e9e430cb9f08ee4feca7345551a9a175c974c338d8a538c98a77b8ac5a32b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54178482"
---
# <a name="deleteaction-resource-type"></a>Tipo de recurso deleteAction

Namespace: microsoft.graph

A presença do recurso **deleteAction** em um [**itemActivity**][activity] indica que a atividade excluiu um item.

>**Observação:** No momento, os registros de atividade do item estão disponíveis apenas SharePoint e OneDrive for Business.

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
  "@type&quot;: &quot;microsoft.graph.deleteAction"
}-->

```json
{
  "name": "string",
  "objectType&quot;: &quot;File | Folder"
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

