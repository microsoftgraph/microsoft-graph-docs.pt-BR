---
title: tipo de recurso updateRecordingStatusOperation
description: Descreve o formato de resposta de uma ação de status de gravação de atualização.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 302ea2c5ce0cfb54168bf936f8c6e5829e0867c7
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/31/2019
ms.locfileid: "40913279"
---
# <a name="updaterecordingstatusoperation-resource-type"></a>tipo de recurso updateRecordingStatusOperation

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Descreve o formato de resposta de uma ação de status de gravação de atualização.

## <a name="properties"></a>Propriedades

| Propriedade            | Tipo                        | Descrição|
|:--------------------|:----------------------------|:-----------------------------------------------------------------------------------|
| clientContext       | String                      | Cadeia de caracteres de contexto de cliente exclusivo. O limite máximo é de 256 caracteres.                              |
| id                  | Cadeia de caracteres                      | Somente leitura.                                                                         |
| resultInfo          | [resultInfo](resultinfo.md) | As informações de resultado. Somente leitura.                                                 |
| status              | String                      | Os valores possíveis são: `notStarted`, `running`, `completed`, `failed`.               |

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.updateRecordingStatusOperation"
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
  "description": "updateRecordingStatusOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
