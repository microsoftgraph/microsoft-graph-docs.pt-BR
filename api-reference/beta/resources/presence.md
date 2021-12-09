---
title: tipo de recurso de presença
description: Contém informações sobre a presença de um usuário, incluindo sua disponibilidade e atividade do usuário.
author: mkhribech
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: cloud-communications
ms.openlocfilehash: 8589be83cc647952676b7f0059c60c1d60778b91
ms.sourcegitcommit: f336c5c49fbcebe55312656aa8b50511fd99a657
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/09/2021
ms.locfileid: "61390987"
---
# <a name="presence-resource-type"></a>tipo de recurso de presença

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Contém informações sobre a presença de um usuário, incluindo sua disponibilidade e atividade do usuário.

> **Observação:** Atualmente, esse recurso só tem suporte para Microsoft Teams usuários.

Esse recurso dá suporte à assinatura para [alterar notificações.](/graph/webhooks)

## <a name="methods"></a>Métodos

| Método                                                                               | Tipo de retorno                                     | Descrição                                                                       |
| :----------------------------------------------------------------------------------- | :---------------------------------------------- | :-------------------------------------------------------------------------------- |
| [Obter presença](../api/presence-get.md)                                               | [presence](../resources/presence.md)            | Obter informações de presença de um usuário.                                                |
| [Obter presença de vários usuários](../api/cloudcommunications-getpresencesbyuserid.md) | [coleção presence](../resources/presence.md) | Obter informações de presença para vários usuários.                                  |
| [Definir presença](../api/presence-setpresence.md)                                       |                                                 | De definir o status de disponibilidade e atividade em [uma sessão de](../api/presence-setpresence.md#presence-sessions) presença de um aplicativo para um usuário. |
| [Presença clara](../api/presence-clearpresence.md)                                   |                                                 | Desmarcar uma sessão de presença de um aplicativo para um usuário.                                       |
| [Definir a presença preferencial do usuário](../api/presence-setuserpreferredpresence.md)           |                                                 | De definir o status de disponibilidade e atividade preferencial para um usuário.                    |
| [Limpar a presença preferencial do usuário](../api/presence-clearuserpreferredpresence.md)       |                                                 | Limpe o status de disponibilidade e atividade preferencial para um usuário.                  |

## <a name="properties"></a>Propriedades

| Relação        | Tipo                                          | Descrição                                                                                                                                                                                                                                                                                    |
| :------------------ | :-------------------------------------------- | :--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| id                  | string                                        | A ID do objeto user                                                                                                                                                                                                                                                                             |
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
