---
title: tipo de recurso workbookChartAxisTitleFormat
description: Representa a formatação do título do eixo do gráfico.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: a676bb28ccce19c7f4293e9fc082a59ec0cfdbb7
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519355"
---
# <a name="workbookchartaxistitleformat-resource-type"></a>tipo de recurso workbookChartAxisTitleFormat

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa a formatação do título do eixo do gráfico.


## <a name="methods"></a>Métodos
Nenhum

## <a name="properties"></a>Propriedades
Nenhuma

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|font|[workbookChartFont](workbookchartfont.md)|Representa os atributos de fonte, como nome, tamanho, cor, etc., do objeto do eixo do gráfico. Somente leitura.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "font"
    ],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartAxisTitleFormat"
}-->

```json
{
  "font": {"@odata.type": "microsoft.graph.workbookChartFont"}
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "ChartAxisTitleFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
