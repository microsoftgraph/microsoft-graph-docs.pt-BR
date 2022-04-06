---
author: daspek
description: Um columnLink em um contentType anexa um columnDefinition de site para esse tipo de conteúdo.
ms.date: 09/12/2017
title: ColumnLink
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: ae75a605f8476b9ec25d5aab5cf50f1bf9508c95
ms.sourcegitcommit: e5d5095e26dca6f434354a0970e789e94ee6afb0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/22/2022
ms.locfileid: "63723525"
---
# <a name="columnlink-resource-type"></a>Tipo de recurso ColumnLink

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um **columnLink** em um [contentType][] anexa um **columnDefinition** de site para esse tipo de conteúdo.

[contentType]: contenttype.md

## <a name="json-representation"></a>Representação JSON

Aqui está uma representação JSON de um recurso **columnLink**.

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.columnLink" } -->

```json
{
  "id": "string",
  "name&quot;: &quot;string"
}
```

## <a name="properties"></a>Propriedades

| Propriedade | Tipo   | Descrição                                   |
| :------- | :----- | :-------------------------------------------- |
| **id**   | string | O identificador exclusivo da coluna.         |
| **name** | string | O nome da coluna desse tipo de conteúdo. |

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
