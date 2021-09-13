---
title: Tipo de recurso rejectJoinResponse
description: Contém uma resposta para rejeitar um participante que tenta ingressar na reunião.
author: yizhenww
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: f16c061d6652f68ca27744d32e1203ef46c1d1fd
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59044241"
---
# <a name="rejectjoinresponse-resource-type"></a>Tipo de recurso rejectJoinResponse

Namespace: microsoft.graph

Contém uma resposta para rejeitar um participante que tenta ingressar na reunião.

Isso tem o mesmo efeito que rejeitar uma notificação de chamada de entrada de registro de política usando [o método reject-call.](../api/call-reject.md) O bot continuará a receber uma notificação de participação de um participante para um novo usuário ingressar até que sua capacidade seja atingida.

## <a name="properties"></a>Propriedades

| Propriedade         | Tipo                            | Descrição                                                                                                                                                  |
| :--------------- | :------------------------------ | :----------------------------------------------------------------------------------------------------------------------------------------------------------- |
| motivo           | String                          | O motivo da rejeição. Os valores possíveis são: `None`, `Busy` e `Forbidden`.                                                                                     |

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
