---
title: Tipo de recurso stopHoldMusicOperation
description: Representa o status de uma operação stopHoldMusic, disparada por uma chamada para a API stopHoldMusic.
author: mkhribech
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: a0a30e783bfbcb08c613b2c0dd80a933d206830e
ms.sourcegitcommit: cbad97d6a8ccb89b1822b30a11cc9b6f2670deda
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/30/2021
ms.locfileid: "60016547"
---
# <a name="stopholdmusicoperation-resource-type"></a>Tipo de recurso stopHoldMusicOperation

Namespace: microsoft.graph

Representa o status de uma [operação stopHoldMusic,](../api/participant-stopholdmusic.md) disparada por uma chamada para a API **stopHoldMusic.** Herda de [commsOperation](commsoperation.md).

## <a name="properties"></a>Propriedades

| Propriedade                       | Tipo                        | Descrição                                                                                                                                       |
| :----------------------------- | :---------------------------| :-------------------------------------------------------------------------------------------------------------------------------------------------|
| clientContext                  | String                      | Herdado **de commsOperation**. Cadeia de caracteres de contexto de cliente exclusiva. Pode ter no máximo 256 caracteres.                                                                               |
| id                             | String                      | Herdado **de commsOperation**. A ID da operação do servidor. Somente leitura.                                                                                            |
| resultInfo                     | [resultInfo](resultinfo.md) | Herdado **de commsOperation**. As informações de resultado.  Somente leitura.                                                                                            |
| status                         | String                      | Herdado **de commsOperation**. Os valores possíveis são: `notStarted`, `running`, `completed`, `failed`. Somente leitura.                                                 |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.stopHoldMusicOperation"
}-->
```json
{
  "clientContext": "String",
  "id": "String (identifier)",
  "resultInfo": { "@odata.type": "microsoft.graph.resultInfo" },
  "status": "notStarted | running | completed | failed"
}
```