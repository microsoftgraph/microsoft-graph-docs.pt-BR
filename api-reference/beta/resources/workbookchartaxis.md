---
title: tipo de recurso workbookChartAxis
description: Representa um único eixo em um gráfico.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 929fd2569067e67af6770b9281bce1d09cd9eca4
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007372"
---
# <a name="workbookchartaxis-resource-type"></a>tipo de recurso workbookChartAxis

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um único eixo em um gráfico.


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Get ChartAxis](../api/chartaxis-get.md) | [workbookChartAxis](workbookchartaxis.md) |Leia as propriedades e os relacionamentos do objeto chartAxis.|
|[Update](../api/chartaxis-update.md) | [workbookChartAxis](workbookchartaxis.md)   |Atualize o objeto ChartAxis. |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
| id       |string   | Identificador exclusivo. Somente leitura.|
|majorUnit|Json|Representa o intervalo entre as duas principais marcas de escala. Pode ser definido como um valor numérico ou uma cadeia de caracteres vazia.  O valor retornado sempre é um número.|
|maximum|Json|Representa o valor máximo no eixo dos valores.  Pode ser definido como um valor numérico ou uma cadeia de caracteres vazia (para valores automáticos de eixo).  O valor retornado sempre é um número.|
|minimum|Json|Representa o valor mínimo no eixo dos valores. Pode ser definido como um valor numérico ou uma cadeia de caracteres vazia (para valores automáticos de eixo).  O valor retornado sempre é um número.|
|minorUnit|Json|Representa o intervalo entre duas marcas de escala secundárias. Pode ser definido como um valor numérico ou uma cadeia de caracteres vazia (para valores automáticos de eixo). O valor retornado sempre é um número.|

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|formato|[workbookChartAxisFormat](workbookchartaxisformat.md)|Representa a formatação de um objeto Chart, que inclui formatação de linha e de fonte. Somente leitura.|
|majorGridlines|[workbookChartGridlines](workbookchartgridlines.md)|Retorna um objeto de linha de grade que representa as principais linhas de grade do eixo especificado. Somente leitura.|
|minorGridlines|[workbookChartGridlines](workbookchartgridlines.md)|Retorna um objeto Gridlines que representa as linhas de grade secundárias do eixo especificado. Somente leitura.|
|title|[workbookChartAxisTitle](workbookchartaxistitle.md)|Representa o título do eixo. Somente leitura.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "title",
    "minorGridlines",
    "majorGridlines",
    "format"
   ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.workbookChartAxis"
}-->

```json
{
  "id": "string",
  "majorUnit": "string",
  "maximum": "string",
  "minimum": "string",
  "minorUnit": "string",
  "format": {"@odata.type": "microsoft.graph.workbookChartAxisFormat"},
  "majorGridlines": {"@odata.type": "microsoft.graph.workbookChartGridlines"},
  "minorGridlines": {"@odata.type": "microsoft.graph.workbookChartGridlines"},
  "title": {"@odata.type": "microsoft.graph.workbookChartAxisTitle"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "ChartAxis resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
