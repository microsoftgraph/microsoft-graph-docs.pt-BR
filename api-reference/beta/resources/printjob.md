---
title: tipo de recurso printJob
description: Representa um trabalho de impressão que foi enfileirado para uma impressora.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 7810c8cd864020c42de4482deea67620950f6cf0
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48726289"
---
# <a name="printjob-resource-type"></a>tipo de recurso printJob

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um trabalho de impressão que foi enfileirado para uma impressora.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Get](../api/printjob-get.md) | [Impressão](printjob.md) | Leia as propriedades e as relações do objeto printJob. |
| [Create](../api/printer-post-jobs.md) | [Impressão](printjob.md) | Criar um novo objeto de trabalho de impressão. |
| [Start](../api/printjob-start.md)|Nenhum|Iniciar o trabalho de impressão.|
| [Cancel](../api/printjob-cancel.md)|Nenhum|Cancele o trabalho de impressão.|
| [Redirecionar (para outra impressora)](../api/printjob-redirect.md) | [Impressão](printjob.md) | Um trabalho de impressão que está na fila da impressora de destino. |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|id|String|O GUID da impressora. Somente leitura.|
|createdDateTime|DateTimeOffset|O DateTimeOffset quando o trabalho foi criado. Somente leitura.|
|status|[printJobStatus](printjobstatus.md)|O status do trabalho de impressão. Somente leitura.|
|configuration|[printJobConfiguration](printJobConfiguration.md)|Um grupo de configurações que uma impressora deve usar para imprimir um trabalho.|
|isfetchable|Edm.Boolean|Se true, o documento pode ser obtido pela impressora.|
|redirectedFrom|Edm.String|Contém a URL do trabalho de origem, se o trabalho foi Redirecionado de outra impressora.|
|redirecionato|Edm.String|Contém a URL do trabalho de destino, se o trabalho foi redirecionado para outra impressora.|

## <a name="relationships"></a>Relações
| Relação | Tipo        | Descrição |
|:-------------|:------------|:------------|
|createdBy|[userIdentity](useridentity.md)| Somente leitura. Anulável.|
|documentos|coleção [AddDocument](printdocument.md)| Somente leitura.|
|tarefas|coleção [multitask](printtask.md)|Uma lista de [multitarefas](printtask.md) que foram acionadas por esse trabalho de impressão.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printJob",
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity"
}-->

```json
{
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "isFetchable": "Boolean",
  "redirectedFrom": "String",
  "redirectedTo": "String",
  "status": {"@odata.type": "microsoft.graph.printJobStatus"},
  "createdBy": {"@odata.type": "microsoft.graph.userIdentity"},
  "configuration": {"@odata.type": "microsoft.graph.printJobConfiguration"},
  "documents": [ {"@odata.type": "microsoft.graph.printDocument"} ]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printJob resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

