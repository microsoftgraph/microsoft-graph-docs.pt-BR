---
title: Tipo de recurso callTranscriptionInfo
description: Representa um único evento DTMF.
author: rzhang
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 27571ad09d6fe29c511b0efa59939dc65074235f9c0c2d4137251687068c47f0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54200793"
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


