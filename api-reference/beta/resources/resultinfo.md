---
title: tipo de recurso resultInfo
description: O tipo resultInfo.
author: VinodRavichandran
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 1e5f6a523a8aca4454cd3355e2a0287fef9fc90d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965366"
---
# <a name="resultinfo-resource-type"></a>tipo de recurso resultInfo

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O tipo resultInfo.

## <a name="properties"></a>Propriedades

| Propriedade | Tipo   | Descrição          |
| :------- | :----- | :------------------  |
| código     | String | O código de resultado.     |
| mensagem  | String | A mensagem.         |
| Subcódigo  | String | O subcódigo do resultado. |

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
  "code": "String",
  "message": "String",
  "subCode": "String"
}
```

## <a name="example-error-result"></a>Exemplo de resultado de erro

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.resultInfo"
}-->
```json
{
  "code": "100",
  "message": "Internal Server Error.",
  "subCode": "20"
}
```

## <a name="example-generic-success-result"></a>Exemplo de resultado genérico de êxito

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.resultInfo"
}-->
```json
{
  "code": "200",
  "message": "",
  "subCode": "0"
}
```

## <a name="example-record-success-result"></a>Resultado de êxito do registro de exemplo

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.resultInfo"
}-->
```json
{
  "code": "200",
  "message": "",
  "subCode": "completedSilenceDetected"
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
