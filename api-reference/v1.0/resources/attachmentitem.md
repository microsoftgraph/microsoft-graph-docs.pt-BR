---
title: Tipo de recurso attachmentItem
description: Representa atributos de um item a ser anexado.
localization_priority: Normal
author: abheek-das
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 385af6c31033ceabf1293c29e9127187cf879d64
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135776"
---
# <a name="attachmentitem-resource-type"></a>Tipo de recurso attachmentItem

Namespace: microsoft.graph

Representa atributos de um item a ser anexado.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|attachmentType|String| O tipo de anexo. Os valores possíveis são: `file`, `item`, `reference`. Obrigatório.|
|contentType|String|A natureza dos dados no anexo. Opcional.|
|isInline|Booliano|`true` se o anexo for embutido; caso contrário, `false`. Opcional.|
|nome|Cadeia de caracteres|O nome de exibição do anexo. Pode ser uma cadeia de caracteres descritiva e não precisa ser o nome de arquivo real. Obrigatório.|
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
