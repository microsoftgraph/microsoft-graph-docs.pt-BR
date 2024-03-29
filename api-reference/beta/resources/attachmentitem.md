---
title: Tipo de recurso attachmentItem
description: Representa atributos de um item a ser anexado.
ms.localizationpriority: medium
author: abheek-das
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 236e2ed7cb26f0c8c5cd3e4ed086ab58f77087d6
ms.sourcegitcommit: 94741ff7f61f20a39dacfa6ce451a77ca02dd68a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/14/2022
ms.locfileid: "62047231"
---
# <a name="attachmentitem-resource-type"></a>Tipo de recurso attachmentItem

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa atributos de um item a ser anexado.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|attachmentType|String| O tipo de anexo. Os valores possíveis são: `file`, `item`, `reference`. Obrigatório.|
|contentId|String| A CID ou a ID de conteúdo do anexo para fazer referência em caso de anexos em linha usando `<img src="cid:contentId">` a marca em mensagens HTML. Opcional.|
|contentType|String|A natureza dos dados no anexo. Opcional.|
|isInline|Booliano|`true` se o anexo for embutido; caso contrário, `false`. Opcional.|
|nome|Cadeia de caracteres|O nome de exibição do anexo. Isso pode ser uma cadeia de caracteres descritiva e não precisa ser o nome de arquivo real. Obrigatório.|
|size|Int64|O comprimento do anexo em bytes. Obrigatório.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "contentId",
    "contentType",
    "isInline"
  ],
  "@odata.type": "microsoft.graph.attachmentItem",
  "baseType": null
}-->

```json
{
  "attachmentType": "String",
  "contentId": "String",
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

