---
title: tipo de recurso printTaskTrigger
description: Determina as condições sob as quais uma nova multitarefa será executada com base no printTaskDefinition associado.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: fc05fe9011d91ac9da5f74a6079537ebfba25160
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48078287"
---
# <a name="printtasktrigger-resource-type"></a>tipo de recurso printTaskTrigger

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Determina a condição sob a qual uma nova [multitarefa](printtask.md) será disparada com base no [printTaskDefinition](printtaskdefinition.md)associado.

Para obter detalhes sobre como usar esse recurso para adicionar suporte à impressão pull à impressão universal, consulte [estender a impressão universal para dar suporte à impressão pull](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [List](../api/printer-list-tasktriggers.md) | coleção [printTaskTrigger](printtasktrigger.md) | Obtenha uma lista de printTaskTriggers associados a uma [impressora](printer.md)específica. |
| [Get](../api/printtasktrigger-get.md) | [printTaskTrigger](printtasktrigger.md) | Obter o printTaskTrigger associado a uma [multitarefa](printtask.md)em particular. |


## <a name="properties"></a>Propriedades
| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|id|Cadeia de caracteres|O identificador do printTaskTrigger. Somente leitura.|
|event|MyEvent|O evento de impressão universal que fará com que [uma nova impressão seja disparada](printtask.md) . Os valores válidos são descritos na tabela a seguir.|

### <a name="printevent-values"></a>valores de MyEvent

|Membro|Valor|Descrição|
|:---|:---|:---|
|jobStarted|,0|Representa um evento que ocorre quando um novo trabalho de impressão é iniciado.|
|unknownFutureValue|1 |Valor de sentinela de enumeração evolvable. Não usar.|

## <a name="relationships"></a>Relacionamentos
| Relação | Tipo        | Descrição |
|:-------------|:------------|:------------|
|definir|[printTaskDefinition](printtaskdefinition.md)|Uma definição abstrata que será usada para criar uma [multitarefa](printtask.md) quando disparado por um evento Print. Somente leitura.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printTaskTrigger",
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity"
}-->

```json
{
  "id": "String (identifier)",
  "event": {"@odata.type": "microsoft.graph.printEvent"},
  "definition": {"@odata.type": "microsoft.graph.printTaskDefinition"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printTaskTrigger resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


