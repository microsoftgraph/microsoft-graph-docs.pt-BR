---
title: Tipo de recurso Filter
description: Gerencia a filtragem da coluna de uma tabela.
localization_priority: Normal
author: ruoyingl
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 0d3204213fe70fa66cd9fac569a5c4629a414a780b65e8e8d6f238b901a4a2ec
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54205819"
---
# <a name="filter-resource-type"></a>Tipo de recurso Filter

Namespace: microsoft.graph

Gerencia a filtragem da coluna de uma tabela.


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Apply](../api/filter-apply.md)|Nenhum|Aplica os critérios de filtro determinados à coluna fornecida.|
|[Clear](../api/filter-clear.md)|Nenhum|Limpa o filtro na coluna determinada.|

## <a name="properties"></a>Propriedades

| Nome | Tipo   |Descrição|
|:---------------|:--------|:----------|
|criteria|[WorkbookFilterCriteria](filtercriteria.md)|O filtro aplicado no momento à coluna fornecida. Somente leitura.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookFilter"
}-->

```json
{
  "criteria": {"@odata.type": "microsoft.graph.workbookFilterCriteria" }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Filter resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

