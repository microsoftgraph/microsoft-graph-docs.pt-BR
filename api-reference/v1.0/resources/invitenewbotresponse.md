---
title: Tipo de recurso inviteNewBotResponse
description: Contém uma resposta a uma solicitação para que uma notificação de participação do participante seja enviada novamente como uma notificação de chamada de entrada para o local desejado.
author: yizhenww
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: cca303fff854fddff56f6bc8ffd30160f390401c
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59084402"
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
