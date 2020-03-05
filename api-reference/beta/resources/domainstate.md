---
title: tipo de recurso domainstate
description: Representa o status de operações assíncronas agendadas em um domínio.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 66d5d5b57cb5ef30054a6187e34caf8713b6e63b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42505802"
---
# <a name="domainstate-resource-type"></a>tipo de recurso domainstate

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o status de operações assíncronas agendadas em um domínio.

## <a name="properties"></a>Propriedades

| Propriedade   | Tipo | Descrição |
|:---------------|:--------|:----------|
| lastActionDateTime | DateTimeOffset | Carimbo de data/hora de quando a última atividade ocorreu. O valor é atualizado quando uma operação é agendada, a tarefa assíncrona é iniciada e quando a operação é concluída. |
| operações | String | Tipo de operação assíncrona. Os valores podem ser *ForceDelete* ou *verificação* |
| status | String | Status atual da operação. <br> *Scheduled* -a operação foi agendada, mas não foi iniciada. <br> *InProgress* – a tarefa foi iniciada e está em andamento. <br> *Failed* -a operação falhou. |

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
  "suppressions": []
}
-->
