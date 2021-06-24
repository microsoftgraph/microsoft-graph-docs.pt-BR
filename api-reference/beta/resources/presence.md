---
title: tipo de recurso de presença
description: Contém informações sobre a presença de um usuário, incluindo sua disponibilidade e atividade do usuário.
author: ananmishr
localization_priority: Normal
doc_type: resourcePageType
ms.prod: cloud-communications
ms.openlocfilehash: 257167fe5b7d417751771650f8e5f03b3dd66296
ms.sourcegitcommit: d586ddb253d27f9ccb621bd128f6a6b4b1933918
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/24/2021
ms.locfileid: "53107687"
---
# <a name="presence-resource-type"></a>tipo de recurso de presença

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Contém informações sobre a presença de um usuário, incluindo sua disponibilidade e atividade do usuário.

> **Observação:** Atualmente, esse recurso só tem suporte para Microsoft Teams usuários.

Esse recurso dá suporte à assinatura para [alterar notificações.](/graph/webhooks)

## <a name="methods"></a>Métodos

| Método                                                                               | Tipo de retorno                                     | Descrição                                      |
| :----------------------------------------------------------------------------------- | :---------------------------------------------- | :----------------------------------------------- |
| [Obter presença](../api/presence-get.md)                                               | [presence](../resources/presence.md)            | Obter informações de presença de um usuário.               |
| [Obter presença de vários usuários](../api/cloudcommunications-getpresencesbyuserid.md) | [coleção presence](../resources/presence.md) | Obter informações de presença para vários usuários. |
| [Definir presença](../api/presence-setpresence.md)                                               |                                                 | Definir a sessão de presença de um aplicativo para um usuário.           |
| [Presença clara](../api/presence-clearpresence.md)                                           |                                                 | Desmarcar a sessão de presença de um aplicativo para um usuário.         |

## <a name="properties"></a>Propriedades

| Relação        | Tipo                                          | Descrição                                                                                                                                                                                                                                                                                    |
| :------------------ | :-------------------------------------------- | :--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| id                  | cadeia de caracteres                                        | A ID do objeto user                                                                                                                                                                                                                                                                             |
| availability        | coleção de cadeias de caracteres                             | As informações de presença base para um usuário. Os valores possíveis `Available` são , , , , , , , `AvailableIdle` ,  `Away` `BeRightBack` `Busy` `BusyIdle` `DoNotDisturb` `Offline` , `PresenceUnknown`                                                                                                           |
| atividade            | coleção de cadeias de caracteres                             | As informações complementares à disponibilidade de um usuário. Os valores `Available` possíveis `Away` são , , , , , , , `BeRightBack` , , , `Busy` , , , `DoNotDisturb` `InACall` , `InAConferenceCall` `Inactive` `InAMeeting` `Offline` `OffWork` `OutOfOffice` `PresenceUnknown` `Presenting` `UrgentInterruptionsOnly` . |
| outOfOfficeSettings | [outOfOfficeSettings](outOfOfficeSettings.md) | As configurações fora do escritório para um usuário.                                                                                                                                                                                                                                                         |

>**Observação:** Para saber mais sobre os diferentes estados de presença, consulte [Presença do usuário em Teams](/microsoftteams/presence-admins). 

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
   "activity":"string",
   "outOfOfficeSettings":{"@odata.type": "#microsoft.graph.outOfOfficeSettings"}
}
```
