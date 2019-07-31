---
title: tipo de recurso workbookFilter
description: Gerencia a filtragem da coluna de uma tabela.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: excel
author: ''
ms.openlocfilehash: f3622a2efd952907214add4343bb5958adebe606
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007120"
---
# <a name="workbookfilter-resource-type"></a>tipo de recurso workbookFilter

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Gerencia a filtragem da coluna de uma tabela.


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Apply](../api/filter-apply.md)|Nenhum|Aplica os critérios de filtro determinados à coluna fornecida.|
|[Clear](../api/filter-clear.md)|Nenhum|Limpa o filtro na coluna determinada.|

## <a name="properties"></a>Propriedades
Nenhuma

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|criteria|[workbookFilterCriteria](workbookfiltercriteria.md)|O filtro aplicado no momento à coluna fornecida. Somente leitura.|


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
     "legacyId"
  ],
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookFilter"
}-->

```json
{
    "criteria": {"@odata.type": "microsoft.graph.workbookFilterCriteria"}
}

```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Filter resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
