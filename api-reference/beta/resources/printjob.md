---
title: Tipo de recurso printJob
description: Representa um trabalho de impressão que foi ensuado para uma impressora.
author: braedenp-msft
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 5124f3123331c4889f5e16110109938e7f264925
ms.sourcegitcommit: 1d2adc4062c8e83d23768682cf66a731bccd313c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/16/2021
ms.locfileid: "49883029"
---
# <a name="printjob-resource-type"></a>Tipo de recurso printJob

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um trabalho de impressão que foi ensuado para uma impressora.

## <a name="methods"></a>Methods

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Get](../api/printjob-get.md) | [printJob](printjob.md) | Leia as propriedades e os relacionamentos do objeto printJob. |
| [Create](../api/printer-post-jobs.md) | [printJob](printjob.md) | Criar um novo objeto de trabalho de impressão. |
| [Start](../api/printjob-start.md)|Nenhum|Iniciar o trabalho de impressão.|
| [Cancel](../api/printjob-cancel.md)|Nenhum|Cancele o trabalho de impressão.|
| Anular**|Nenhum|Anula o trabalho de impressão.|
| [Redirecionar (para outra impressora)](../api/printjob-redirect.md) | [printJob](printjob.md) | Um trabalho de impressão que está na fila para a impressora de destino. |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|id|String|O GUID da impressora. Somente leitura.|
|createdDateTime|DateTimeOffset|DateTimeOffset quando o trabalho foi criado. Somente leitura.|
|status|[printJobStatus](printjobstatus.md)|O status do trabalho de impressão. Somente leitura.|
|configuração|[printJobConfiguration](printJobConfiguration.md)|Um grupo de configurações que uma impressora deve usar para imprimir um trabalho.|
|isFetchable|Edm.Boolean|Se verdadeiro, o documento pode ser buscado pela impressora.|
|redirectedFrom|Edm.String|Contém a URL do trabalho de origem, se o trabalho tiver sido redirecionado de outra impressora.|
|redirectedTo|Edm.String|Contém a URL do trabalho de destino, se o trabalho tiver sido redirecionado para outra impressora.|

## <a name="relationships"></a>Relações
| Relação | Tipo        | Descrição |
|:-------------|:------------|:------------|
|createdBy|[userIdentity](useridentity.md)| Somente leitura. Anulável.|
|documentos|[Coleção printDocument](printdocument.md)| Somente leitura.|
|tarefas|[Coleção printTask](printtask.md)|Uma lista de [printTasks](printtask.md) que foram disparadas por esse trabalho de impressão.|

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

