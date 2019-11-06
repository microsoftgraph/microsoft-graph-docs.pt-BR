---
title: tipo de recurso playPromptOperation
description: A operação playPrompt para obter o resultado da ação playPrompt.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 84b54fbce830f5b505decee7e2d25618700728b3
ms.sourcegitcommit: 9bddc0b7746383e8d05ce50d163af3f4196f12a6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/06/2019
ms.locfileid: "38006575"
---
# <a name="playpromptoperation-resource-type"></a>tipo de recurso playPromptOperation

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

A operação playPrompt para obter o resultado da ação playPrompt.

## <a name="properties"></a>Propriedades

| Propriedade            | Tipo                        | Descrição|
|:--------------------|:----------------------------|:-----------------------------------------------------------------------------------|
| clientContext       | String                      | Cadeia de caracteres de contexto de cliente exclusivo. O limite máximo é de 256 caracteres.                              |
| completionReason    | String                      | Os valores possíveis são: `unknown`, `completedSuccessfully`, `mediaOperationCanceled`. |
| id                  | Cadeia de caracteres                      | Somente leitura.                                                                         |
| resultInfo          | [resultInfo](resultinfo.md) | As informações de resultado. Somente leitura.                                |
| status              | String                      | Os valores possíveis são: `notStarted`, `running`, `completed`, `failed`.               |

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.playPromptOperation"
}-->
```json
{
  "clientContext": "String",
  "completionReason": "unknown | completedSuccessfully | mediaOperationCanceled",
  "id": "String (identifier)",
  "resultInfo": {"@odata.type": "#microsoft.graph.resultInfo"},
  "status": "notStarted | running | completed | failed"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "playPromptOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
