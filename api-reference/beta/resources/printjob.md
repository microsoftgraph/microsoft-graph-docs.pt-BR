---
title: tipo de recurso printJob
description: Representa um trabalho de impressão que foi enfileirado para uma impressora.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 2c0a1bdb4ec3ebe3c87b5b40595d30cf9108c5bf
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48048733"
---
# <a name="printjob-resource-type"></a>tipo de recurso printJob

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um trabalho de impressão que foi enfileirado para uma impressora.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Get](../api/printjob-get.md) | [Impressão](printjob.md) | Leia as propriedades e as relações do objeto printJob. |
| [Criar](../api/printer-post-jobs.md) | [Impressão](printjob.md) | Criar um novo objeto de trabalho de impressão. |
| [Start](../api/printjob-startprintjob.md)|Nenhum|Iniciar o trabalho de impressão.|
| [Cancel](../api/printjob-cancelprintjob.md)|Nenhum|Cancele o trabalho de impressão.|
| [Redirecionar (para outra impressora)](../api/printjob-redirect.md) | [Impressão](printjob.md) | Um trabalho de impressão que está na fila da impressora de destino. |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|id|Cadeia de caracteres|O GUID da impressora. Somente leitura.|
|createdDateTime|DateTimeOffset|O DateTimeOffset quando o trabalho foi criado. Somente leitura.|
|status|[printJobStatus](printjobstatus.md)|O status do trabalho de impressão. Somente leitura.|

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
  "status": {"@odata.type": "microsoft.graph.printJobStatus"},
  "createdBy": {"@odata.type": "microsoft.graph.userIdentity"},
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

