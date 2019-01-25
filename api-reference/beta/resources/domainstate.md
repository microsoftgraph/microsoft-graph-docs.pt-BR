---
title: Tipo de recurso domainState
description: Representa o status das operações assíncronas agendadas em um domínio.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 39ded8e4ff3458ebaceea09b3003d0bd14be36cf
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512973"
---
# <a name="domainstate-resource-type"></a>Tipo de recurso domainState

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o status das operações assíncronas agendadas em um domínio.

## <a name="properties"></a>Propriedades

| Propriedade   | Tipo | Descrição |
|:---------------|:--------|:----------|
| lastActionDateTime | DateTimeOffset | O carimbo de data/hora de quando a última atividade ocorreu. O valor é atualizado quando uma operação é agendada, a tarefa assíncrona começa e quando a operação é concluída. |
| operação | String | Tipo de operação assíncrona. Os valores podem ser *ForceDelete* ou *Verification* |
| status | Cadeia de caracteres | Status atual da operação. <br> *Scheduled* – A operação foi agendada, mas não foi iniciada. <br> *InProgress* – A tarefa foi iniciada e está em andamento. <br> *Failed* - A operação falhou. |

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domainState"
}-->

```json
{
  "lastActionDateTime": "String (timestamp)",
  "operation": "String",
  "status": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "domainState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/domainstate.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
