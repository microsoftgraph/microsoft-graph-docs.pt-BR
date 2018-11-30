---
title: Tipo de recurso Filter
description: Gerencia a filtragem da coluna de uma tabela.
ms.openlocfilehash: 272b4ea0ee91c25ea845217512a12e33b08ed7b8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27005076"
---
# <a name="filter-resource-type"></a>Tipo de recurso Filter

Gerencia a filtragem da coluna de uma tabela.


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Aplicar](../api/filter-apply.md)|Nenhum|Aplica os critérios de filtro determinados à coluna fornecida.|
|[Clear](../api/filter-clear.md)|Nenhum|Limpa o filtro na coluna determinada.|

## <a name="properties"></a>Propriedades

| Nome | Tipo   |Descrição|
|:---------------|:--------|:----------|
|critérios|[WorkbookFilterCriteria](filtercriteria.md)|O filtro aplicado no momento à coluna fornecida. Somente leitura.|

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