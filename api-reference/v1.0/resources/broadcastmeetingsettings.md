---
title: Tipo de recurso broadcastMeetingSettings
description: Configurações relacionado a um evento ao vivo
author: mkhribech
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 0a78c4665c42bf11c983bbf24aa72a93cdff323a
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59031709"
---
# <a name="broadcastmeetingsettings-resource-type"></a>Tipo de recurso broadcastMeetingSettings

Namespace: microsoft.graph

Configurações relacionado a um evento ao vivo.

## <a name="properties"></a>Propriedades

| Propriedade                   | Tipo                                                         | Descrição                                                                                 |
|----------------------------|--------------------------------------------------------------|---------------------------------------------------------------------------------------------|
| allowedAudience            | [broadcastMeetingAudience](#broadcastmeetingaudience-values) | Define quem pode participar do evento ao vivo. Os valores possíveis são listados na tabela a seguir.     |
| isRecordingEnabled         | Booliano                                                      | Indica se a gravação está habilitada para esse evento ao vivo. O valor padrão é `false`.       |
| isAttendeeReportEnabled    | Booliano                                                      | Indica se o relatório do participante está habilitado para este evento ao vivo. O valor padrão é `false`. |
| isQuestionAndAnswerEnabled | Boolean                                                      | Indica se O&A está habilitado para este evento ao vivo. O valor padrão é `false`.             |
| isVideoOnDemandEnabled     | Booliano                                                      | Indica se o vídeo sob demanda está habilitado para esse evento ao vivo. O valor padrão é `false`. |

### <a name="broadcastmeetingaudience-values"></a>valores broadcastMeetingAudience

| Valor              | Descrição                                                       |
|--------------------|-------------------------------------------------------------------|
| everyone           | O evento ao vivo será aberto a qualquer pessoa. Esse é o valor padrão. |
| organization       | Todos em sua organização podem participar do evento ao vivo.                     |
| roleIsAttendee     | Somente as pessoas especificadas podem participar do evento ao vivo.                |
| unknownFutureValue | Valor de sentinela de enumeração evolvável. Não usar.                 |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.broadcastMeetingSettings"
}-->
```json
{
  "allowedAudience": "everyone | organization | roleIsAttendee | unknownFutureValue",
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
