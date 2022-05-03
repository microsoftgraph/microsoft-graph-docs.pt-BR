---
title: Tipo de recurso printTaskTrigger
description: Determina as condições sob as quais uma nova printTask será executada com base na printTaskDefinition associada.
author: braedenp-msft
ms.localizationpriority: medium
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 461a3ed348cfb0dc4329d641944ddf39f9e4a56d
ms.sourcegitcommit: 267e3baf545c8dc71ba2ab69497e3ec369379f43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/03/2022
ms.locfileid: "65176350"
---
# <a name="printtasktrigger-resource-type"></a>Tipo de recurso printTaskTrigger

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Determina a condição sob a qual uma [nova printTask](printtask.md) será disparada com base na [printTaskDefinition associada](printtaskdefinition.md).

Para obter detalhes sobre como usar esse recurso para adicionar suporte de impressão pull à Impressão Universal, consulte Estendendo Impressão Universal para dar suporte [à impressão pull](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [List](../api/printer-list-tasktriggers.md) | [Coleção printTaskTrigger](printtasktrigger.md) | Obtenha uma lista de printTaskTriggers associados a uma impressora [específica](printer.md). |
| [Get](../api/printtasktrigger-get.md) | [printTaskTrigger](printtasktrigger.md) | Obtenha um printTaskTrigger específico associado a uma impressora [específica](printer.md).|


## <a name="properties"></a>Propriedades
| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|id|Cadeia de caracteres|O identificador de printTaskTrigger. Somente leitura.|
|event|printEvent|O evento de Impressão Universal que fará com que uma [nova printTask](printtask.md) seja disparada. Os valores válidos são descritos na tabela a seguir.|

### <a name="printevent-values"></a>Valores printEvent

|Membro|Valor|Descrição|
|:---|:---|:---|
|jobStarted|0|Representa um evento que ocorre quando um novo trabalho de impressão é iniciado.|
|unknownFutureValue|1|Valor de sentinel de enumeração evolvável. Não usar.|

## <a name="relationships"></a>Relações
| Relação | Tipo        | Descrição |
|:-------------|:------------|:------------|
|Definição|[printTaskDefinition](printtaskdefinition.md)|Uma definição abstrata que será usada para criar [uma printTask](printtask.md) quando disparada por um evento de impressão. Somente leitura.|

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


