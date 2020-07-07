---
title: tipo de recurso Presence
description: Contém informações sobre a presença de um usuário, incluindo a disponibilidade e a atividade do usuário.
author: ananmishr
localization_priority: Normal
doc_type: resourcePageType
ms.prod: cloud-communications
ms.openlocfilehash: 3a185d3f38fb1437205d99be103974f78eb49d6b
ms.sourcegitcommit: 67433748b69541727185fc1f32ed356718bf6ff1
ms.contentlocale: pt-BR
ms.lasthandoff: 07/07/2020
ms.locfileid: "45050915"
---
# <a name="presence-resource-type"></a>tipo de recurso Presence

Namespace: microsoft.graph

Contém informações sobre a presença de um usuário, incluindo a disponibilidade e a atividade do usuário.

> **Observação:** No momento, esse recurso só tem suporte para usuários do Microsoft Teams.

Esse recurso oferece suporte à assinatura de [alteração de notificações](/graph/webhooks).

## <a name="methods"></a>Métodos

| Método                                                            | Tipo de retorno                                       | Descrição                                  |
|:------------------------------------------------------------------|:--------------------------------------------------|:---------------------------------------------|
| [Obter presença](../api/presence-get.md)     | [presença](../resources/presence.md)     | Obtenha as informações de presença de um usuário.
| [Obter presença de vários usuários](../api/cloudcommunications-getpresencesbyuserid.md)    |  coleção [Presence](../resources/presence.md)     |  Obtenha as informações de presença de vários usuários.      |


## <a name="properties"></a>Propriedades

| Relação        | Tipo                                                 | Descrição                                                         |
|:--------------------|:-----------------------------------------------------|:--------------------------------------------------------------------|
|id    |  string     |  A ID de objeto de usuário   |
|availability    |  coleção de cadeias de caracteres   |   As informações de presença básicas de um usuário. Os valores possíveis são,,,,, `Available` `AvailableIdle` ,, `Away` `BeRightBack` `Busy` `BusyIdle` `DoNotDisturb` `Offline` ,`PresenceUnknown`  |
|atividade    |  coleção de cadeias de caracteres      |    As informações complementares para a disponibilidade de um usuário. Os valores possíveis são,,,,, `Available` `Away` `BeRightBack` `Busy` `DoNotDisturb` `InACall` `InAConferenceCall` , `Inactive` , `InAMeeting` , `Offline` , `OffWork` , `OutOfOffice` , `PresenceUnknown` , `Presenting` , `UrgentInterruptionsOnly` .       |

>**Observação:** Para saber mais sobre os diferentes Estados de presença, confira [presença do usuário no Microsoft Teams](https://docs.microsoft.com/microsoftteams/presence-admins). 

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  ],
  "@odata.type": "microsoft.graph.presence"
}-->
```json
{
   "id":"string",
   "availability":"string",
   "activity":"string"
}
```
