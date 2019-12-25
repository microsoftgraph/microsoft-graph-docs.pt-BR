---
title: tipo de recurso resultInfo
description: Isso contém informações específicas sobre o resultado de êxito e falha.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 39027ecf949860d9ffa757a95839ae7fd8184a27
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40865644"
---
# <a name="resultinfo-resource-type"></a>tipo de recurso resultInfo

Isso contém informações específicas sobre o resultado de êxito e falha. 

O código especifica se o resultado é um êxito ou uma falha genérica. Se o código for 2xx, ele será um sucesso, se for um 4xx um erro de cliente e, se for 5xx, é um erro de servidor.

Os subcódigos fornecem informações complementares relacionadas ao tipo de êxito ou falha (por exemplo, uma transferência de chamada foi bem-sucedida)


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
