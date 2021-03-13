---
title: Tipo de recurso domainState
description: Representa o status de operações assíncronas agendadas em um domínio.
author: adimitui
localization_priority: Normal
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 9ab9a4af3109e35cd1022b4d62869ce3bb034100
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761181"
---
# <a name="domainstate-resource-type"></a>Tipo de recurso domainState

Namespace: microsoft.graph

Representa o status de operações assíncronas agendadas em um domínio.

## <a name="properties"></a>Propriedades

| Propriedade   | Tipo | Descrição |
|:---------------|:--------|:----------|
| lastActionDateTime | DateTimeOffset | Timestamp para quando ocorreu a última atividade. O valor é atualizado quando uma operação é agendada, a tarefa assíncrona é iniciada e quando a operação é concluída. |
| operation | String | Tipo de operação assíncrona. Os valores podem ser *ForceDelete* ou *Verification* |
| status | String | Status atual da operação. <br> *Agendado* - A operação foi agendada, mas não foi iniciada. <br> *InProgress* - A tarefa foi iniciada e está em andamento. <br> *Falha* - Falha na operação. |

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
<!-- {
  "type": "#page.annotation",
  "description": "domainState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

