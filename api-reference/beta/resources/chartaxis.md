---
title: Tipo de recurso ChartAxis
description: Representa um único eixo em um gráfico.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 6cb780272887b6a9b637bbec24b68b37db93657e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32535548"
---
# <a name="chartaxis-resource-type"></a>Tipo de recurso ChartAxis

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um único eixo em um gráfico.


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Get ChartAxis](../api/chartaxis-get.md) | [ChartAxis](chartaxis.md) |Leia as propriedades e os relacionamentos do objeto chartAxis.|
|[Update](../api/chartaxis-update.md) | [ChartAxis](chartaxis.md)   |Atualize o objeto ChartAxis. |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|majorUnit|objeto|Representa o intervalo entre as duas principais marcas de escala. Pode ser definido como um valor numérico ou uma cadeia de caracteres vazia.  O valor retornado sempre é um número.|
|maximum|objeto|Representa o valor máximo no eixo dos valores.  Pode ser definido como um valor numérico ou uma cadeia de caracteres vazia (para valores automáticos de eixo).  O valor retornado sempre é um número.|
|minimum|objeto|Representa o valor mínimo no eixo dos valores. Pode ser definido como um valor numérico ou uma cadeia de caracteres vazia (para valores automáticos de eixo).  O valor retornado sempre é um número.|
|minorUnit|objeto|Representa o intervalo entre duas marcas de escala secundárias. Pode ser definido como um valor numérico ou uma cadeia de caracteres vazia (para valores automáticos de eixo). O valor retornado sempre é um número.|

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|format|[ChartAxisFormat](chartaxisformat.md)|Representa a formatação de um objeto Chart, que inclui formatação de linha e de fonte. Somente leitura.|
|majorGridlines|[ChartGridlines](chartgridlines.md)|Retorna um objeto de linha de grade que representa as principais linhas de grade do eixo especificado. Somente leitura.|
|minorGridlines|[ChartGridlines](chartgridlines.md)|Retorna um objeto Gridlines que representa as linhas de grade secundárias do eixo especificado. Somente leitura.|
|title|[ChartAxisTitle](chartaxistitle.md)|Representa o título do eixo. Somente leitura.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chartaxis"
}-->

```json
{
  "majorUnit": "string",
  "maximum": "string",
  "minimum": "string",
  "minorUnit": "string"
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
  "suppressions": [
    "Error: /api-reference/beta/resources/chartaxis.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
