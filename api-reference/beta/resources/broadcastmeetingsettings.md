---
title: Tipo de recurso broadcastMeetingSettings
description: Configurações relacionado a um evento Teams ao vivo
author: mkhribech
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 36e5778761ac792e84096fd54f48c766e524149d
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/03/2021
ms.locfileid: "60696529"
---
# <a name="broadcastmeetingsettings-resource-type"></a>Tipo de recurso broadcastMeetingSettings

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Configurações relacionado a um [evento Microsoft Teams ao vivo.](/microsoftteams/teams-live-events/what-are-teams-live-events)

## <a name="properties"></a>Propriedades

| Propriedade                   | Tipo                     | Descrição                                                                     |
| -------------------------- | ------------------------ | ------------------------------------------------------------------------------- |
| allowedAudience            | [broadcastMeetingAudience](#broadcastmeetingaudience-values) | Define quem pode ingressar no evento Teams ao vivo. Os valores possíveis são listados na tabela a seguir. |
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
