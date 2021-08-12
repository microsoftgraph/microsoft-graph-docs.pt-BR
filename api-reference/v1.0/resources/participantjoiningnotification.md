---
title: Tipo de recurso participantJoiningNotification
description: Contém detalhes sobre o participante baseado em política ingressar em uma chamada.
author: yizhenww
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: c3cac84db6b08a26c35bd01294bc476b2859bcd4eef2d61db9a4d65dc1ad9af1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54152331"
---
# <a name="participantjoiningnotification-resource-type"></a>Tipo de recurso participantJoiningNotification

Namespace: microsoft.graph

Contém detalhes sobre o participante baseado em política ingressar em uma chamada.

No cenário [de](/microsoftteams/teams-recording-policy)registro baseado em política , antes de um participante na política ingressar em uma chamada, um será enviado para o bot associado à política que tem capacidade disponível para lidar com o `participantJoiningNotification` novo participante.

Um [participanteJoiningResponse](participantjoiningResponse.md) na carga de resposta é esperado do bot.

## <a name="properties"></a>Propriedades
| Propriedade       | Tipo            | Descrição                                                        |
| -------------- | --------------  | -------------------------------------------                        |
| call           | [call](call.md) | O objeto call que contém detalhes sobre o evento de participação do participante. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.participantJoiningNotification"
}-->
```json
{
  "call": {"@odata.type": "#microsoft.graph.call"}
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "participantJoiningNotification resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
