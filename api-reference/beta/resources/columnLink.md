---
author: daspek
description: Um columnLink em um contentType anexa um columnDefinition de site para esse tipo de conteúdo.
ms.date: 09/12/2017
title: ColumnLink
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 4add6ac0edc401815d8072371ce0faca48d5852b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36012940"
---
# <a name="columnlink-resource-type"></a>Tipo de recurso ColumnLink

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
| **id**        | string | O identificador exclusivo da coluna.
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
