---
title: Tipo de recurso playPromptOperation
description: A operação playPrompt para obter o resultado da ação playPrompt.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: ab75f0346bf0739a08e2608d1348ccf52030982fb0a75e0d0670f20debc362fe
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54251847"
---
# <a name="playpromptoperation-resource-type"></a>Tipo de recurso playPromptOperation

Namespace: microsoft.graph

A operação playPrompt para obter o resultado da ação playPrompt.

## <a name="properties"></a>Propriedades

| Propriedade            | Tipo                        | Descrição|
|:--------------------|:----------------------------|:-----------------------------------------------------------------------------------|
| clientContext       | String                      | Cadeia de caracteres de contexto de cliente exclusiva. O limite máximo é 256 caracteres.                              |
| id                  | String                      | Somente leitura.                                                                         |
| resultInfo          | [resultInfo](resultinfo.md) | As informações de resultado. Apenas leitura.                                |
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

