---
title: tipo de recurso resultInfo
description: Contém informações de resultado específicas de êxito e falha.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: aa55f8cdcb7ca4639aa4975a28ae2bcbcd625588
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521079"
---
# <a name="resultinfo-resource-type"></a>tipo de recurso resultInfo

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Contém informações de resultado específicas de êxito e falha. 

O código especifica se o resultado é um êxito ou uma falha genérica. 

Os subcódigos fornecem informações complementares relacionadas ao tipo de sucesso ou falha (por exemplo, uma transferência de chamada foi bem-sucedida).


## <a name="properties"></a>Propriedades

| Propriedade | Tipo   | Descrição          |
| :------- | :----- | :------------------  |
| código     | Int32 | O código de resultado.     |
| mensagem  | String | A mensagem.         |
| subcódigo  | Int32 | O subcódigo do resultado. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.resultInfo"
}-->
```json
{
  "code": 0,
  "message": "String",
  "subcode": 0
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "resultInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
