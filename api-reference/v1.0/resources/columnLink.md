---
author: daspek
ms.author: dspektor
ms.date: 09/12/2017
title: ColumnLink
ms.openlocfilehash: ef7fef6fb6ca35f1117433b452de0841691282a0
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/28/2017
---
# <a name="columnlink-resource-type"></a>Tipo de recurso ColumnLink

Um **columnLink** em um [contentType][] anexa um **columnDefinition** de site para esse tipo de conteúdo.

[contentType]: contentType.md

## <a name="json-representation"></a>Representação JSON

Aqui está uma representação JSON de um recurso **columnLink**.
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.columnLink" } -->

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
