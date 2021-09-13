---
title: Tipo de recurso participantLeftNotification
description: Contém detalhes sobre o participante baseado em política que deixou a chamada.
author: yizhenww
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: cdd3bb5b41fcd37c03b1814e7226ce84e6edafa1
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59036050"
---
# <a name="participantleftnotification-resource-type"></a>Tipo de recurso participantLeftNotification

Namespace: microsoft.graph

Contém detalhes sobre o participante baseado em política que deixou a chamada.

No cenário [de](/microsoftteams/teams-recording-policy) gravação baseado em Política, quando um participante gerenciado pela chamada de bot sair da reunião, um será enviado para o bot para notificar o bot com detalhes do evento à esquerda do `participantLeftNotification` participante.

## <a name="properties"></a>Propriedades
| Propriedade       | Tipo            | Descrição                                                        |
| -------------- | --------------  | -------------------------------------------                        |
| call           | [call](call.md) | O objeto call que contém detalhes sobre o evento de participação do participante. |
| participantId  | Cadeia de caracteres          | ID do participante na política que saiu da reunião.        |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.participantLeftNotification"
}-->
```json
{
  "participantId": "String",
  "call": {"@odata.type": "#microsoft.graph.call"}
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "participantLeftNotification resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
