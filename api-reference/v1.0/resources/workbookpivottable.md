---
title: tipo de recurso de tabela dinâmica
description: Representa uma Tabela Dinâmica do Excel.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: fb67920598d883a126c18cdf8acdfb1b38d9014a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48015131"
---
# <a name="pivottable-resource-type"></a>tipo de recurso de tabela dinâmica

Namespace: microsoft.graph

Representa uma Tabela Dinâmica do Excel.

## <a name="methods"></a>Methods

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Get workbookPivotTable](../api/workbookpivottable-get.md) | [workbookPivotTable](workbookpivottable.md) |Leia as propriedades e relacionamentos do objeto workbookPivotTable.|
|[Refresh](../api/workbookpivottable-refresh.md)|Nenhum|Atualiza a Tabela Dinâmica. |
|[Refreshall](../api/workbookpivottable-refreshall.md)|Nenhum|Atualização de todas as tabelas dentro de uma determinada planilha. Observe que esta ação está disponível somente na coleção de tabela dinâmica.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|id|String| Id da Tabela Dinâmica.   Somente leitura.|
|name|String|Nome da Tabela Dinâmica.    |

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|planilha|[WorkbookWorksheet](worksheet.md)| A planilha que contém a Tabela Dinâmica atual. Somente leitura.   |

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookPivotTable"
}-->

```json
{
  "id": "String (identifier)",
  "name": "String"
}

```

