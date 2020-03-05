---
title: tipo de recurso unmuteParticipantOperation
description: Descreve o formato de resposta de uma chamada operação de desativação de participantes.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: d9ebb8d749f8cbe6ce01711ca6a0c36b134e8369
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519593"
---
# <a name="unmuteparticipantoperation-resource-type"></a>tipo de recurso unmuteParticipantOperation

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Descreve o formato de resposta de uma chamada operação de desativação de participantes.

## <a name="properties"></a>Propriedades

| Propriedade                       | Tipo                        | Descrição                                                                                                                                       |
| :----------------------------- | :---------------------------| :-------------------------------------------------------------------------------------------------------------------------------------------------|
| clientContext                  | String                      | Cadeia de caracteres de contexto de cliente exclusivo. Pode ter um máximo de 256 caracteres.                                                                               |
| id                             | Cadeia de caracteres                      | A ID da operação do servidor. Somente leitura.                                                                                            |
| resultInfo                     | [resultInfo](resultinfo.md) | As informações de resultado.  Somente leitura.                                                                                            |
| status                         | String                      | Os valores possíveis são: `notStarted`, `running`, `completed`, `failed`. Somente leitura.                                                 |

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.unmuteParticipantOperation"
}-->
```json
{
  "clientContext": "String",
  "id": "String (identifier)",
  "resultInfo": {"@odata.type": "#microsoft.graph.resultInfo"},
  "status": "notStarted | running | completed | failed"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "unmuteParticipantOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
