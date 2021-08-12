---
title: Tipo de recurso callTranscriptionInfo
description: Representa um único evento DTMF.
author: rzhang
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: d6d3afe17198d8c9eaa4df396500582d1bc52deeb5e5acb721131a7737dac55e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54178532"
---
# <a name="calltranscriptioninfo-resource-type"></a>Tipo de recurso callTranscriptionInfo

Namespace: microsoft.graph

Representa um único evento DTMF.

## <a name="properties"></a>Propriedades

| Propriedade       | Tipo    | Descrição|
|:---------------|:--------|:----------|
| state | Cadeia de caracteres | Os valores possíveis são: `notStarted`, `active`, `inactive`. |
| lastModifiedDateTime | DateTime | O tempo de modificação de estado em UTC. |

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

