---
title: Tipo de recurso printTaskStatus
description: Representa o status de execução atual de uma printTask.
author: braedenp-msft
ms.localizationpriority: medium
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: c484ef988e7452096d63fe103a6c45a8d22d06ff
ms.sourcegitcommit: 267e3baf545c8dc71ba2ab69497e3ec369379f43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/03/2022
ms.locfileid: "65176325"
---
# <a name="printtaskstatus-resource-type"></a>Tipo de recurso printTaskStatus

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o status de execução atual de [uma printTask](printtask.md). 

>**Nota:** Os aplicativos que registram gatilhos de tarefa são responsáveis por atualizar os status da tarefa quando o processamento for concluído, a menos que o trabalho de impressão relacionado tenha sido redirecionado para outra impressora.

Para obter detalhes sobre como usar esse recurso para adicionar suporte de impressão pull à Impressão Universal, consulte Estendendo Impressão Universal para dar suporte [à impressão pull](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|state|printTaskProcessingState|O estado de processamento atual da [printTask](printtask.md). Os valores válidos são descritos na tabela a seguir.|
|descrição|Cadeia de caracteres|Uma descrição legível por humanos do estado de processamento atual da [printTask](printtask.md).|

### <a name="printtaskprocessingstate-values"></a>Valores printTaskProcessingState

|Membro|Valor|Descrição|
|:---|:---|:---|
|Pendente|0|A execução da tarefa está pendente.|
|Processamento|1|A execução da tarefa está em andamento.|
|Concluído|2|A execução da tarefa foi concluída.|
|Abortado|3|A execução da tarefa foi anulada.|
|unknownFutureValue|4|Valor de sentinel de enumeração evolvável. Não usar.|

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


