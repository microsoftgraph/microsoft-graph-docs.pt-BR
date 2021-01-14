---
title: Tipo de recurso broadcastMeetingSettings
description: Configurações relacionadas a um evento ao vivo
author: frankpeng7
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 42ac666817b6f259dd888e479939216fc3e39c6c
ms.sourcegitcommit: dbbf77c732ae8d982e59865432b9b6147002a30a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/14/2021
ms.locfileid: "49866246"
---
# <a name="broadcastmeetingsettings-resource-type"></a>Tipo de recurso broadcastMeetingSettings

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Configurações relacionadas a um evento ao vivo.

> [!IMPORTANT]
> Essa API não valida configurações de eventos ao vivo gerenciadas por [política.](/microsoftteams/teams-live-events/set-teams-live-events-policies-using-powershell)
> Por exemplo, se um administrador definir uma política de evento ao vivo usando , os usuários serão impedidos de definir permissões de evento ao vivo no cliente do Teams, mas poderão criar um evento ao vivo por meio do Microsoft Graph definindo `Set-CsTeamsMeetingBroadcastPolicy -Identity Global -BroadcastAttendeeVisibility EveryoneInCompany` `public` **allowedAudience** como `everyone` . 

## <a name="properties"></a>Propriedades

| Propriedade                   | Tipo                     | Descrição                                                                     |
| -------------------------- | ------------------------ | ------------------------------------------------------------------------------- |
| allowedAudience            | broadcastMeetingAudience | Define quem pode ingressar no evento ao vivo. Os valores possíveis estão listados na tabela a seguir. |
| isRecordingEnabled         | Boolean                  | Indica se a gravação está habilitada para este evento ao vivo. O valor padrão é `false`.          |
| isAttendeeReportEnabled    | Boolean                  | Indica se o relatório de participantes está habilitado para este evento ao vivo. O valor padrão é `false`.    |
| isQuestionAndAnswerEnabled | Boolean                  | Indica se as&A estão habilitadas para este evento ao vivo. O valor padrão é `false`.                |
| isVideoOnDemandEnabled     | Boolean                  | Indica se o vídeo sob demanda está habilitado para este evento ao vivo. O valor padrão é `false`.    |

### <a name="broadcastmeetingaudience-values"></a>Valores de broadcastMeetingAudience

| Valor              | Descrição                                                       |
| ------------------ | ----------------------------------------------------------------- |
| everyone           | O evento ao vivo será aberto para qualquer pessoa. Esse é o valor padrão. |
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
