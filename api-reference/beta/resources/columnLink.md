---
author: daspek
description: Um columnLink em um contentType anexa um columnDefinition de site para esse tipo de conteúdo.
ms.date: 09/12/2017
title: ColumnLink
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 2c4da6165a33caa50de38788a927c4bb0c54fd90
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507632"
---
# <a name="columnlink-resource-type"></a>Tipo de recurso ColumnLink

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um **columnLink** em um [contentType][] anexa um **columnDefinition** de site para esse tipo de conteúdo.

[contentType]: contenttype.md

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
| **id**        | cadeia de caracteres | O identificador exclusivo da coluna.
| **name**      | string | O nome da coluna desse tipo de conteúdo.

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ColumnLink",
  "suppressions": []
}
-->
