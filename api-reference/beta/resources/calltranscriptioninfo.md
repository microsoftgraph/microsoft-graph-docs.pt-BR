---
title: Tipo de recurso callTranscriptionInfo
description: Representa um único evento DTMF.
author: rzhang
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 1597d86fa37e55ec8c5a205a24688c101c8838e0
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59023826"
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


