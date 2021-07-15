---
title: Tipo de recurso inviteNewBotResponse
description: Contém uma resposta a uma solicitação para que uma notificação de participação do participante seja enviada novamente como uma notificação de chamada de entrada para o local desejado.
author: yizhenww
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 675b7cd1df35b25e3414f36a4dd04e389e05b192
ms.sourcegitcommit: 6d247f44a6ee4d8515c3863ee8a2683163c9f829
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/14/2021
ms.locfileid: "53430183"
---
# <a name="invitenewbotresponse-resource-type"></a>Tipo de recurso inviteNewBotResponse

Namespace: microsoft.graph

Contém uma resposta a uma solicitação para que uma notificação de participação do participante seja enviada novamente como uma notificação de chamada de entrada para o local desejado.

## <a name="properties"></a>Propriedades

| Propriedade         | Tipo                            | Descrição                                                                                                                                                  |
| :--------------- | :------------------------------ | :----------------------------------------------------------------------------------------------------------------------------------------------------------- |
| inviteUri        | Cadeia de caracteres                          | URI para receber nova notificação de chamada de entrada.                                                                                                                |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.inviteNewBotResponse"
}-->
```json
{
  "inviteUri": "uri" 
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "inviteNewBotResponse resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
