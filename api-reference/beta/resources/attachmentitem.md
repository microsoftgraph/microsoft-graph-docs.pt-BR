---
title: tipo de recurso attachmentItem
description: Representa os atributos de um item a ser anexado.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: fa739af74f00142405ecb536346639d3a2ca9f60
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508154"
---
# <a name="attachmentitem-resource-type"></a>tipo de recurso attachmentItem

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa os atributos de um item a ser anexado.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|attachmentType|String| O tipo de anexo. Os valores possíveis são: `file`, `item`, `reference`. Obrigatório.|
|contentType|String|A natureza dos dados no anexo. Opcional.|
|isInline|Booliano|`true` se o anexo for embutido; caso contrário, `false`. Opcional.|
|nome|Cadeia de caracteres|O nome de exibição do anexo. Pode ser uma cadeia de caracteres descritiva e não precisa ser o nome real do arquivo. Obrigatório.|
|size|Int64|O comprimento do anexo em bytes. Obrigatório.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "contentType",
    "isInline"
  ],
  "@odata.type": "microsoft.graph.attachmentItem",
  "baseType": null
}-->

```json
{
  "attachmentType": "String",
  "contentType": "String",
  "isInline": true,
  "name": "String",
  "size": 1024
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "attachmentItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->