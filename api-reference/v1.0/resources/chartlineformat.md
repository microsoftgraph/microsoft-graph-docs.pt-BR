---
title: Tipo de recurso ChartLineFormat
description: Encapsula as opções de formatação dos elementos de linha.
author: lumine2008
ms.localizationpriority: medium
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: b60d588de64d5ba28f2b6985c0e4862e876fe025
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59062807"
---
# <a name="chartlineformat-resource-type"></a>Tipo de recurso ChartLineFormat

Namespace: microsoft.graph

Encapsula as opções de formatação dos elementos de linha.


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Get ChartLineFormat](../api/chartlineformat-get.md) | [WorkbookChartLineFormat](chartlineformat.md) |Leia as propriedades e os relacionamentos do objeto chartLineFormat.|
|[Update](../api/chartlineformat-update.md) | [WorkbookChartLineFormat](chartlineformat.md) |Atualize o objeto ChartLineFormat. |
|[Clear](../api/chartlineformat-clear.md)|Nenhum|Limpe a formatação da linha de um elemento do gráfico.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|color|string|Código de cores HTML que representa a cor das linhas no gráfico.|

## <a name="relationships"></a>Relações
Nenhum


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.workbookChartLineFormat"
}-->

```json
{
  "color": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartLineFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

