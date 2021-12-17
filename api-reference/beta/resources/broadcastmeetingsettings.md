---
title: Tipo de recurso broadcastMeetingSettings
description: Representa configurações relacionadas a um evento ao vivo Microsoft Teams.
author: mkhribech
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: c91dda07a2a339bdee40e5ea2f953c2eab65ad98
ms.sourcegitcommit: 1a607ea5bee096944e0fea14167d372f1ff652f6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/16/2021
ms.locfileid: "61545354"
---
# <a name="broadcastmeetingsettings-resource-type"></a>Tipo de recurso broadcastMeetingSettings

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa configurações relacionadas a [um evento ao](/microsoftteams/teams-live-events/what-are-teams-live-events) vivo em Microsoft Teams.

## <a name="properties"></a>Propriedades

| Propriedade                   | Tipo                     | Descrição                                                                     |
| -------------------------- | ------------------------ | ------------------------------------------------------------------------------- |
| allowedAudience            | [broadcastMeetingAudience](#broadcastmeetingaudience-values) | Define quem pode ingressar no evento Teams ao vivo. Os valores possíveis são listados na tabela a seguir. |
| legendas | [broadcastMeetingCaptionSettings](../resources/broadcastmeetingcaptionsettings.md) | Configurações de legenda de um evento Teams ao vivo. |
| isRecordingEnabled         | Booliano                  | Indica se a gravação está habilitada para esse Teams ao vivo. O valor padrão é `false`.          |
| isAttendeeReportEnabled    | Booliano                  | Indica se o relatório do participante está habilitado para este evento Teams ao vivo. O valor padrão é `false`.    |
| isQuestionAndAnswerEnabled | Booliano                  | Indica se a Q&A está habilitada para este evento Teams ao vivo. O valor padrão é `false`.                |
| isVideoOnDemandEnabled     | Booliano                  | Indica se o vídeo sob demanda está habilitado para esse evento Teams ao vivo. O valor padrão é `false`.    |

### <a name="broadcastmeetingaudience-values"></a>valores broadcastMeetingAudience

| Valor              | Descrição                                                       |
| ------------------ | ----------------------------------------------------------------- |
| everyone           | Esse Teams ao vivo será aberto a qualquer pessoa. Esse é o valor padrão. |
| organização       | Todos em sua organização podem participar desse evento Teams ao vivo.                     |
| roleIsAttendee     | Somente as pessoas especificadas podem participar desse evento Teams ao vivo.                |
| unknownFutureValue | Valor de sentinela de enumeração evolvável. Não usar.  |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.broadcastMeetingSettings"
}-->
```json
{
  "@odata.type": "#microsoft.graph.broadcastMeetingSettings",
  "allowedAudience": "String",
  "isRecordingEnabled": "Boolean",
  "isAttendeeReportEnabled": "Boolean",
  "isQuestionAndAnswerEnabled": "Boolean",
  "isVideoOnDemandEnabled": "Boolean",
  "captions": {
    "@odata.type": "microsoft.graph.broadcastMeetingCaptionSettings"
  }
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
