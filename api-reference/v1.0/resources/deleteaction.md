---
author: daspek
title: Tipo de recurso deleteAction
description: O objeto deleteAction fornece informações sobre a exclusão de um item.
ms.localizationpriority: medium
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: e11bf7783bc9c59fe5779c9605acbb4c9e1fb451
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59104233"
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
| objectType    | cadeia de caracteres | `File` ou `Folder` , dependendo do tipo do item excluído.


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

