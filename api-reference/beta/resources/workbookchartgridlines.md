---
title: tipo de recurso workbookChartGridlines
description: Representa linhas de grade principais ou secundárias em um eixo do gráfico.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: bf2b481b3b60b7cf5893a1c7ab6e2f168c7cc1ca
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964011"
---
# <a name="workbookchartgridlines-resource-type"></a>tipo de recurso workbookChartGridlines

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa linhas de grade principais ou secundárias em um eixo do gráfico.


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Obter workbookChartGridlines](../api/chartgridlines-get.md) | [workbookChartGridlines](workbookchartgridlines.md) |Leia as propriedades e os relacionamentos do objeto chartGridlines.|
|[Update](../api/chartgridlines-update.md) | [workbookChartGridlines](workbookchartgridlines.md)    |Atualize o objeto ChartGridlines. |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|visible|booliano|Valor booliano que determina se as linhas de grade do eixo ficam visíveis ou não.|

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|formato|[workbookChartGridlinesFormat](workbookchartgridlinesformat.md)|Representa a formatação de linhas de grade do gráfico. Somente leitura.|

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
<!--
{
  "type": "#page.annotation",
  "description": "ChartGridlines resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
