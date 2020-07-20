---
title: tipo de recurso printTaskStatus
description: Representa o status de execução atual de uma multitarefa.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: c5d46cd0c8d14b6dc07873bc503d024928e2b2e3
ms.sourcegitcommit: 8a74c06be9c41390331ca1717efedc5b5a244db5
ms.translationtype: Auto
ms.contentlocale: pt-BR
ms.lasthandoff: 07/09/2020
ms.locfileid: "45091547"
---
# <a name="printtaskstatus-resource-type"></a>tipo de recurso printTaskStatus

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o status de execução atual de uma [multitarefa](printtask.md). 

>**Observação:** Os aplicativos que registram gatilhos de tarefa são responsáveis por atualizar os status da tarefa quando o processamento for concluído, a menos que o trabalho de impressão relacionado tenha sido Redirecionado para outra impressora.

Para obter detalhes sobre como usar esse recurso para adicionar suporte à impressão pull à impressão universal, consulte [estender a impressão universal para dar suporte à impressão pull](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|state|printTaskProcessingState|O estado de processamento atual da [multitarefa](printtask.md). Os valores válidos são descritos na tabela a seguir.|
|description|String|Uma descrição legível do estado atual de processamento da [tarefa](printtask.md).|

### <a name="printtaskprocessingstate-values"></a>valores de printTaskProcessingState

|Membro|Valor|Descrição|
|:---|:---|:---|
|função|,0|A execução da tarefa está pendente.|
|processe|1 |A execução da tarefa está em andamento.|
|Completed|2 |A execução da tarefa foi concluída.|
|anulada|3 |A execução da tarefa foi anulada.|
|unknownFutureValue|4 |Valor de sentinela de enumeração evolvable. Não usar.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printTaskStatus"
}-->

```json
{
  "state": {"@odata.type": "microsoft.graph.printTaskProcessingState"},
  "description": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printTaskStatus resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
