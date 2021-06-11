---
title: Tipo de recurso broadcastMeetingSettings
description: Configurações relacionado a um evento ao vivo
author: mkhribech
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 1de814ee520d1dbf8d0ea6ba1270c6893a07d2cd
ms.sourcegitcommit: 7abb0672a38a6d9b11a2e0d2cc221222cb8358bb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2021
ms.locfileid: "52896687"
---
# <a name="broadcastmeetingsettings-resource-type"></a>Tipo de recurso broadcastMeetingSettings

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Configurações relacionado a um evento ao vivo.

> [!CAUTION]
> Esta API não valida as configurações de evento ao vivo gerenciadas pela [política](/microsoftteams/teams-live-events/set-teams-live-events-policies-using-powershell).
> Por exemplo, se um administrador definir uma política de evento ao vivo usando , os usuários serão impedidos de definir permissões de evento ao vivo para em seu cliente Teams, mas poderão criar um evento ao vivo por meio do Microsoft Graph definindo `Set-CsTeamsMeetingBroadcastPolicy -Identity Global -BroadcastAttendeeVisibility EveryoneInCompany` `public` **allowedAudience** como `everyone` .

## <a name="properties"></a>Propriedades

| Propriedade                   | Tipo                     | Descrição                                                                     |
| -------------------------- | ------------------------ | ------------------------------------------------------------------------------- |
| allowedAudience            | [broadcastMeetingAudience](#broadcastmeetingaudience-values) | Define quem pode participar do evento ao vivo. Os valores possíveis são listados na tabela a seguir. |
| isRecordingEnabled         | Boolean                  | Indica se a gravação está habilitada para esse evento ao vivo. O valor padrão é `false`.          |
| isAttendeeReportEnabled    | Boolean                  | Indica se o relatório do participante está habilitado para este evento ao vivo. O valor padrão é `false`.    |
| isQuestionAndAnswerEnabled | Boolean                  | Indica se O&A está habilitado para este evento ao vivo. O valor padrão é `false`.                |
| isVideoOnDemandEnabled     | Boolean                  | Indica se o vídeo sob demanda está habilitado para esse evento ao vivo. O valor padrão é `false`.    |

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
