---
title: Tipo de recurso rejectJoinResponse
description: Contém uma resposta para rejeitar um participante que tenta ingressar na reunião.
author: yizhenww
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: c917b2c5ba0ed273af1c8e89c78b07a80d6c45fc
ms.sourcegitcommit: 6d247f44a6ee4d8515c3863ee8a2683163c9f829
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/14/2021
ms.locfileid: "53428854"
---
# <a name="rejectjoinresponse-resource-type"></a>Tipo de recurso rejectJoinResponse

Namespace: microsoft.graph

Contém uma resposta para rejeitar um participante que tenta ingressar na reunião.

Isso tem o mesmo efeito que rejeitar uma notificação de chamada de entrada de registro de política usando [o método reject-call.](../api/call-reject.md) O bot continuará a receber uma notificação de participação de um participante para um novo usuário ingressar até que sua capacidade seja atingida.

## <a name="properties"></a>Propriedades

| Propriedade         | Tipo                            | Descrição                                                                                                                                                  |
| :--------------- | :------------------------------ | :----------------------------------------------------------------------------------------------------------------------------------------------------------- |
| motivo           | Cadeia de caracteres                          | O motivo da rejeição. Os valores possíveis são: `None`, `Busy` e `Forbidden`.                                                                                     |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.rejectJoinResponse"
}-->
```json
{
  "reason": "None | Busy | Forbidden" 
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "rejectJoinResponse resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
