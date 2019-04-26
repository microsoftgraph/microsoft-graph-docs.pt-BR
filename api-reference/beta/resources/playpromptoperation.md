---
title: tipo de recurso playPromptOperation
description: A operação playPrompt para obter o resultado da ação playPrompt.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: a6ecdb06c910923d35f9d36590ad09fd7835fccb
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563655"
---
# <a name="playpromptoperation-resource-type"></a>tipo de recurso playPromptOperation

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

A operação playPrompt para obter o resultado da ação playPrompt.

## <a name="properties"></a>Propriedades

| Propriedade            | Tipo                        | Descrição|
|:--------------------|:----------------------------|:-----------------------------------------------------------------------------------|
| clientContext       | String                      | O contexto do cliente.                                                                |
| completionReason    | String                      | Os valores possíveis são: `unknown`, `completedSuccessfully`, `mediaOperationCanceled`. |
| createdDateTime     | DateTimeOffset              | A hora de início da operação.                                                   |
| id                  | Cadeia de caracteres                      | Somente leitura.                                                                         |
| lastActionDateTime  | DateTimeOffset              | A hora da última ação da operação.                                      |
| resultInfo          | [resultInfo](resultInfo.md) | As informações de resultado. Somente leitura. Servidor gerado.                               |
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
  "createdDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "lastActionDateTime": "String (timestamp)",
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
