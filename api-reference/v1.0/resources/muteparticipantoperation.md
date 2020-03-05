---
title: Tipo de recurso MuteParticipantOperation
description: Descreve o formato de resposta de uma operação do participante sem som de chamada.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: eb85ea8e1759dc948f764b391e25a51b97090566
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447371"
---
# <a name="muteparticipantoperation-resource-type"></a>Tipo de recurso MuteParticipantOperation

Namespace: Microsoft. Graph

Descreve o formato de resposta de uma operação do participante sem som de chamada.

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
  "@odata.type": "microsoft.graph.muteParticipantOperation"
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
  "description": "muteParticipantOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
