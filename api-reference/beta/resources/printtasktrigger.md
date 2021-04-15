---
title: Tipo de recurso printTaskTrigger
description: Determina as condições em que um novo printTask será executado com base na printTaskDefinition associada.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: de2da4f94894d9744fdfdd302b310251cd91fdb3
ms.sourcegitcommit: 412507a3c3a8e407fcc43b7cd227d4db35791f58
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2021
ms.locfileid: "51766319"
---
# <a name="printtasktrigger-resource-type"></a>Tipo de recurso printTaskTrigger

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Determina a condição na qual um [novo printTask](printtask.md) será acionado com base na [impressão associadaTaskDefinition](printtaskdefinition.md).

Para obter detalhes sobre como usar esse recurso para adicionar suporte à impressão pull à Impressão Universal, consulte [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [List](../api/printer-list-tasktriggers.md) | [Coleção printTaskTrigger](printtasktrigger.md) | Obter uma lista de printTaskTriggers associados a uma impressora [específica.](printer.md) |
| [Get](../api/printtasktrigger-get.md) | [printTaskTrigger](printtasktrigger.md) | Obter uma determinada printTaskTrigger associada a uma impressora [específica.](printer.md)|


## <a name="properties"></a>Propriedades
| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|id|String|O identificador printTaskTrigger. Somente leitura.|
|event|printEvent|O evento Impressão Universal que fará com que um [novo printTask](printtask.md) seja acionado. Os valores válidos são descritos na tabela a seguir.|

### <a name="printevent-values"></a>valores printEvent

|Membro|Valor|Descrição|
|:---|:---|:---|
|jobStarted|0|Representa um evento que ocorre quando um novo trabalho de impressão é iniciado.|
|unknownFutureValue|1|Valor de sentinela de enumeração evolvável. Não usar.|

## <a name="relationships"></a>Relações
| Relação | Tipo        | Descrição |
|:-------------|:------------|:------------|
|definition|[printTaskDefinition](printtaskdefinition.md)|Uma definição abstrata que será usada para criar [uma printTask](printtask.md) quando disparada por um evento de impressão. Somente leitura.|

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


