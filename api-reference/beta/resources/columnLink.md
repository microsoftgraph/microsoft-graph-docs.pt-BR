---
author: daspek
description: Um columnLink em um contentType anexa um columnDefinition de site para esse tipo de conteúdo.
ms.date: 09/12/2017
title: ColumnLink
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: sites-and-lists
ms.openlocfilehash: 8bf46496209b62748c82e46ca52ec7e7e80ded7c
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/08/2022
ms.locfileid: "65944945"
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
| **id**   | cadeia de caracteres | O identificador exclusivo da coluna.         |
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
