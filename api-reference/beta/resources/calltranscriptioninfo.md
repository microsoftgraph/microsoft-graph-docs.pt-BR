---
title: tipo de recurso callTranscriptionInfo
description: Representa um único evento DTMF.
author: rzhang
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 0f2f91b8aadfd9f819e87eff839090aa37166cf2
ms.sourcegitcommit: ae2e4b8963edcdcc8ce572c06a531db4769d7779
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/29/2020
ms.locfileid: "47312205"
---
# <a name="calltranscriptioninfo-resource-type"></a>tipo de recurso callTranscriptionInfo

Namespace: microsoft.graph

Representa um único evento DTMF.

## <a name="properties"></a>Propriedades

| Propriedade       | Tipo    | Descrição|
|:---------------|:--------|:----------|
| estado | String | Os valores possíveis são: `notStarted`, `active`, `inactive`. |
| lastModifiedDateTime | DateTime | O horário de modificação do estado em UTC. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  ],
  "@odata.type": "microsoft.graph.callTranscriptionInfo"
}-->
```json
{
  "state": "notStarted | active | inactive",
  "lastModifiedDateTime": "String (timestamp)"
}
```
