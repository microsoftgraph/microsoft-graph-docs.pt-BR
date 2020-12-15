---
title: tipo de recurso Presence
description: Contém informações sobre a presença de um usuário, incluindo a disponibilidade e a atividade do usuário.
author: elvinyang-msft
localization_priority: Normal
doc_type: resourcePageType
ms.prod: cloud-communications
ms.openlocfilehash: 1122e14c91a8562757434e4bd36e267ed70790dd
ms.sourcegitcommit: 86d427ac670ebc3fdcf8e06541218bb74d39279d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/15/2020
ms.locfileid: "49675958"
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
|availability    |  coleção de cadeias de caracteres   |   As informações de presença básicas de um usuário. Os valores possíveis são,,,,, `Available` `AvailableIdle` ,,  `Away` `BeRightBack` `Busy` `BusyIdle` `DoNotDisturb` `Offline` , `PresenceUnknown`  |
|atividade    |  coleção de cadeias de caracteres      |    As informações complementares para a disponibilidade de um usuário. Os valores possíveis são,,,,, `Available` `Away` `BeRightBack` `Busy` `DoNotDisturb` `InACall` `InAConferenceCall` , `Inactive` , `InAMeeting` , `Offline` , `OffWork` , `OutOfOffice` , `PresenceUnknown` , `Presenting` , `UrgentInterruptionsOnly` .       |

>**Observação:** Para saber mais sobre os diferentes Estados de presença, confira [presença do usuário no Microsoft Teams](/microsoftteams/presence-admins). 

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
