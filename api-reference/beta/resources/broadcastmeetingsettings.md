---
title: Tipo de recurso broadcastMeetingSettings
description: Configurações relacionadas a um evento ao vivo
author: jsandoval-msft
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: f199a82ee90d6848cb68d670d49d7af1c1d2c739
ms.sourcegitcommit: 6e7d9987a255f1bee04f196a4a7e37f56621bfb8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/22/2021
ms.locfileid: "51944111"
---
# <a name="broadcastmeetingsettings-resource-type"></a>Tipo de recurso broadcastMeetingSettings

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Configurações relacionadas a um evento ao vivo.

> [!CAUTION]
> Esta API não valida as configurações de evento ao vivo gerenciadas pela [política](/microsoftteams/teams-live-events/set-teams-live-events-policies-using-powershell).
> Por exemplo, se um administrador definir uma política de evento ao vivo usando , os usuários serão impedidos de definir permissões de evento ao vivo no cliente do Teams, mas poderão criar um evento ao vivo por meio do Microsoft Graph definindo `Set-CsTeamsMeetingBroadcastPolicy -Identity Global -BroadcastAttendeeVisibility EveryoneInCompany` `public` **allowedAudience** como `everyone` .

## <a name="properties"></a>Propriedades

| Propriedade                   | Tipo                     | Descrição                                                                     |
| -------------------------- | ------------------------ | ------------------------------------------------------------------------------- |
| allowedAudience            | [broadcastMeetingAudience](#broadcastmeetingaudience-values) | Define quem pode participar do evento ao vivo. Os valores possíveis são listados na tabela a seguir. |
| isRecordingEnabled         | Booliano                  | Indica se a gravação está habilitada para esse evento ao vivo. O valor padrão é `false`.          |
| isAttendeeReportEnabled    | Booliano                  | Indica se o relatório do participante está habilitado para este evento ao vivo. O valor padrão é `false`.    |
| isQuestionAndAnswerEnabled | Booliano                  | Indica se O&A está habilitado para este evento ao vivo. O valor padrão é `false`.                |
| isVideoOnDemandEnabled     | Booliano                  | Indica se o vídeo sob demanda está habilitado para esse evento ao vivo. O valor padrão é `false`.    |

### <a name="broadcastmeetingaudience-values"></a>valores broadcastMeetingAudience

| Valor              | Descrição                                                       |
| ------------------ | ----------------------------------------------------------------- |
| everyone           | O evento ao vivo será aberto a qualquer pessoa. Esse é o valor padrão. |
| organization       | Todos em sua organização podem participar do evento ao vivo.                     |
| roleIsAttendee     | Somente as pessoas especificadas podem participar do evento ao vivo.                |
| unknownFutureValue | Valor futuro desconhecido.                                             |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.broadcastMeetingSettings"
}-->
```json
{
  "allowedAudience": "String",
  "isRecordingEnabled": "Boolean",
  "isAttendeeReportEnabled": "Boolean",
  "isQuestionAndAnswerEnabled": "Boolean",
  "isVideoOnDemandEnabled": "Boolean"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "broadcastSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
