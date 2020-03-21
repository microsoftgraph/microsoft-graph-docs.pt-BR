---
title: tipo de recurso printJob
description: Representa um trabalho de impressão que foi enfileirado para uma impressora.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 5eff75fba2c9993275c277877fedec7705021c49
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/21/2020
ms.locfileid: "42895478"
---
# <a name="printjob-resource-type"></a>tipo de recurso printJob

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um trabalho de impressão que foi enfileirado para uma impressora.

## <a name="methods"></a>Methods

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Get](../api/printjob-get.md) | [Impressão](printjob.md) | Leia as propriedades e as relações do objeto printJob. |
| [Create](../api/printer-post-jobs.md) | [Impressão](printjob.md) | Criar um novo objeto de trabalho de impressão. |
| [Start](../api/printjob-startprintjob.md)|Nenhum|Inicie o trabalho de impressão.|
| [Cancel](../api/printjob-cancelprintjob.md)|Nenhum|Cancele o trabalho de impressão.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|id|String|O GUID da impressora. Somente leitura.|
|createdDateTime|DateTimeOffset|O DateTimeOffset quando o trabalho foi criado. Somente leitura.|
|status|[printJobStatus](printjobstatus.md)|O status do trabalho de impressão. Somente leitura.|

## <a name="relationships"></a>Relacionamento
| Relação | Tipo        | Descrição |
|:-------------|:------------|:------------|
|createdBy|[userIdentity](useridentity.md)| Somente leitura. Anulável.|
|documentos|coleção [AddDocument](printdocument.md)| Somente leitura.|

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