---
title: tipo de recurso de playPromptOperation
description: A operação playPrompt para obter o resultado da ação playPrompt.
author: VinodRavichandran
ms.openlocfilehash: d63b8f6cfa96706104cd7baaa08475974b12ca13
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380949"
---
# <a name="playpromptoperation-resource-type"></a>tipo de recurso de playPromptOperation

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

A operação playPrompt para obter o resultado da ação playPrompt.

## <a name="properties"></a>Propriedades

| Propriedade	            | Tipo                        | Descrição|
|:--------------------|:----------------------------|:-----------------------------------------------------------------------------------|
| clientContext       | String                      | O contexto de cliente.                                                                |
| completionReason    | String                      | Os valores possíveis são: `unknown`, `completedSuccessfully`, `mediaOperationCanceled`. |
| createdDateTime     | DateTimeOffset              | A hora de início da operação.                                                   |
| id                  | String                      | Somente leitura.                                                                         |
| lastActionDateTime  | DateTimeOffset              | A hora da última ação da operação.                                      |
| resultInfo          | [resultInfo](resultInfo.md) | As informações de resultado. Somente leitura. Servidor foi gerado.                               |
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
<!-- {
  "type": "#page.annotation",
  "description": "playPromptOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
