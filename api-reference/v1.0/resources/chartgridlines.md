---
title: Tipo de recurso ChartGridlines
description: Representa linhas de grade principais ou secundárias em um eixo do gráfico.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 5d97e1e6664c142a835b8649bc3ec5194bccfe7d85f2658809344dde2c593d67
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54155173"
---
# <a name="chartgridlines-resource-type"></a>Tipo de recurso ChartGridlines

Namespace: microsoft.graph

Representa linhas de grade principais ou secundárias em um eixo do gráfico.


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Get ChartGridlines](../api/chartgridlines-get.md) | [WorkbookChartGridlines](chartgridlines.md) |Leia as propriedades e os relacionamentos do objeto chartGridlines.|
|[Update](../api/chartgridlines-update.md) | [WorkbookChartGridlines](chartgridlines.md)    |Atualize o objeto ChartGridlines. |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|visible|booliano|Valor booliano que determina se as linhas de grade do eixo ficam visíveis ou não.|

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|formato|[WorkbookChartGridlinesFormat](chartgridlinesformat.md)|Representa a formatação de linhas de grade do gráfico. Somente leitura.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookChartGridlines"
}-->

```json
{
  "visible": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartGridlines resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

