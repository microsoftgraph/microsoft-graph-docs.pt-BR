---
author: daspek
ms.date: 09/12/2017
title: ColumnLink
ms.localizationpriority: medium
description: Um columnLink em um contentType anexa um columnDefinition de site para esse tipo de conteúdo.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 1ad2a7397c18ad8be17a5e5bb27c25ecc84dffa6
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59113718"
---
# <a name="columnlink-resource-type"></a>Tipo de recurso ColumnLink

Namespace: microsoft.graph

Um **columnLink** em um [contentType][] anexa um **columnDefinition** de site para esse tipo de conteúdo.

[contentType]: contenttype.md

## <a name="json-representation"></a>Representação JSON

Aqui está uma representação JSON de um recurso **columnLink**.
<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.columnLink" } -->

```json
{
  "id": "string",
  "name&quot;: &quot;string"
}
```

## <a name="properties"></a>Propriedades

| Nome da propriedade | Tipo   | Descrição
|:--------------|:-------|:----------------------------------------------------
| **id**        | cadeia de caracteres | O identificador exclusivo da coluna.
| **name**      | string | O nome da coluna desse tipo de conteúdo.

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath&quot;: &quot;Resources/ColumnLink"
} -->

