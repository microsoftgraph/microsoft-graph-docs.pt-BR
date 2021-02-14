---
author: daspek
ms.date: 09/12/2017
title: ColumnLink
localization_priority: Normal
description: Um columnLink em um contentType anexa um columnDefinition de site para esse tipo de conteúdo.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 4087d97dfec976560bac7c8949d34fd962308950
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/14/2021
ms.locfileid: "50240574"
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
  "name": "string"
}
```

## <a name="properties"></a>Propriedades

| Nome da propriedade | Tipo   | Descrição
|:--------------|:-------|:----------------------------------------------------
| **id**        | string | O identificador exclusivo da coluna.
| **name**      | string | O nome da coluna desse tipo de conteúdo.

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ColumnLink"
} -->

