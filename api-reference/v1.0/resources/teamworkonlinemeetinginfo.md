---
title: Tipo de recurso teamworkOnlineMeetingInfo
description: Representa detalhes sobre uma reunião online Microsoft Teams.
author: jecha
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: ac6dab85a12cdb339bb6527a6c1c436285c1ea75
ms.sourcegitcommit: 4c8444b732b8d6d0de8a95f6666c42095f146266
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/08/2022
ms.locfileid: "62443258"
---
# <a name="teamworkonlinemeetinginfo-resource-type"></a>Tipo de recurso teamworkOnlineMeetingInfo

Namespace: microsoft.graph

Representa detalhes sobre uma reunião online Microsoft Teams.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|calendarEventId|String|O identificador do evento de calendário associado à reunião.|
|joinWebUrl|Cadeia de caracteres|A URL que os usuários clicam para ingressar ou identificar exclusivamente a reunião.|
|organizer|[teamworkUserIdentity](teamworkuseridentity.md)|O organizador da reunião.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamworkOnlineMeetingInfo"
}
-->
``` json
{
  "calendarEventId": "string",
  "joinWebUrl": "string",
  "organizer": {"@odata.type": "microsoft.graph.teamworkUserIdentity"}
}
```

## <a name="see-also"></a>Confira também
- [Chat](chat.md)
