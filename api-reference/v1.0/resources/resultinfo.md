---
title: Tipo de recurso resultInfo
description: Isso contém informações de resultados específicas de sucesso e falha.
author: ananmishr
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 89ac770d9ace4a35365e1c215e00c51e1d060bdd
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59113536"
---
# <a name="resultinfo-resource-type"></a>Tipo de recurso resultInfo

Namespace: microsoft.graph

Isso contém informações de resultados específicas de sucesso e falha. 

O código especifica se o resultado é um sucesso genérico ou uma falha. Se o código for 2xxx, será um sucesso, se for um 4xxx, será um erro do cliente e, se for 5xxx, será um erro de servidor.

Os sub-códigos fornecem informações complementares relacionadas ao tipo de sucesso ou falha (por exemplo, uma transferência de chamada foi bem-sucedida)


## <a name="properties"></a>Propriedades

| Propriedade | Tipo   | Descrição          |
| :------- | :----- | :------------------  |
| código     | Int32 | O código de resultado.     |
| mensagem  | String | A mensagem.         |
| subcódigo  | Int32 | O subcódigo de resultado. |

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

