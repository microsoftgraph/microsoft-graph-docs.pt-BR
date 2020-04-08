---
title: tipo de recurso domainstate
description: Representa o status de operações assíncronas agendadas em um domínio.
author: adimitui
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 86c5bc7fa987b137b7e11fe9ff825939e95d4426
ms.sourcegitcommit: 11503211a31ea17f4e577c21ec36d364184c0580
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/08/2020
ms.locfileid: "43181747"
---
# <a name="domainstate-resource-type"></a>tipo de recurso domainstate

Namespace: microsoft.graph

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
