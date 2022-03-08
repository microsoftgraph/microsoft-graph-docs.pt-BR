---
title: tipo de recurso de presença
description: Contém informações sobre a presença de um usuário, incluindo sua disponibilidade e atividade do usuário.
author: mkhribech
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: cloud-communications
ms.openlocfilehash: 4743cef5b2772f636d7c40118a11e886839acc95
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63334013"
---
# <a name="presence-resource-type"></a>tipo de recurso de presença

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Contém informações sobre a presença de um usuário, incluindo sua disponibilidade e atividade do usuário.

> **Observação:** Atualmente, esse recurso só tem suporte para Microsoft Teams usuários.

Esse recurso dá suporte à assinatura para [alterar notificações](/graph/webhooks).

## <a name="methods"></a>Methods

| Método                                                                               | Tipo de retorno                                     | Descrição                                                                       |
| :----------------------------------------------------------------------------------- | :---------------------------------------------- | :-------------------------------------------------------------------------------- |
| [Obter presença](../api/presence-get.md)                                               | [presence](../resources/presence.md)            | Obter informações de presença de um usuário.                                                |
| [Obter presença de vários usuários](../api/cloudcommunications-getpresencesbyuserid.md) | [coleção presence](../resources/presence.md) | Obter informações de presença para vários usuários.                                  |
| [Definir presença](../api/presence-setpresence.md)                                       |                                                 | De definir o status de disponibilidade e atividade em [uma sessão de](../api/presence-setpresence.md#presence-sessions) presença de um aplicativo para um usuário. |
| [Presença clara](../api/presence-clearpresence.md)                                   |                                                 | Desmarcar uma sessão de presença de um aplicativo para um usuário.                                       |
| [Definir a presença preferencial do usuário](../api/presence-setuserpreferredpresence.md)           |                                                 | De definir o status de disponibilidade e atividade preferencial para um usuário.                    |
| [Limpar a presença preferencial do usuário](../api/presence-clearuserpreferredpresence.md)       |                                                 | Limpe o status de disponibilidade e atividade preferencial para um usuário.                  |

## <a name="properties"></a>Propriedades

| Propriedade        | Tipo                                          | Descrição                                                                                                                                                                                                                                                                                    |
| :------------------ | :-------------------------------------------- | :--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| id                  | cadeia de caracteres                                        | A ID do objeto user                                                                                                                                                                                                                                                                             |
| availability        | coleção de cadeias de caracteres                             | As informações de presença base para um usuário. Os valores possíveis `Available`são , `AvailableIdle``Away`, , `BeRightBack`, `Busy`, `BusyIdle`, `DoNotDisturb`, , `Offline`,`PresenceUnknown`                                                                                                           |
| atividade            | coleção de cadeias de caracteres                             | As informações complementares à disponibilidade de um usuário. Os valores possíveis `Available`são , `BeRightBack``Away`, , `Busy`, `DoNotDisturb`, `InACall`, `InAConferenceCall`, `Inactive`, `Offline``InAMeeting`, , `OffWork`,`OutOfOffice`, `PresenceUnknown`,, ,`Presenting`, `UrgentInterruptionsOnly`. |
| outOfOfficeSettings | [outOfOfficeSettings](outOfOfficeSettings.md) | As configurações fora do escritório para um usuário.                                                                                                                                                                                                                                                         |

>**Observação:** Para saber mais sobre os diferentes estados de presença, consulte [Presença do usuário no Teams](/microsoftteams/presence-admins). 

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
