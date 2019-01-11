---
title: Tipo de recurso ChartAxisTitle
description: Representa o título de um eixo do gráfico.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: a78219e5833f7f85cde571dc984959b642ebe4d4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27894177"
---
# <a name="chartaxistitle-resource-type"></a>Tipo de recurso ChartAxisTitle

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Representa o título de um eixo do gráfico.


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Get ChartAxisTitle](../api/chartaxistitle-get.md) | [ChartAxisTitle](chartaxistitle.md) |Recupere as propriedades e os relacionamentos do objeto chartAxisTitle.|
|[Update](../api/chartaxistitle-update.md) | [ChartAxisTitle](chartaxistitle.md)    |Atualize o objeto ChartAxisTitle. |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|texto|string|Representa o título do eixo.|
|visible|booliano|Um booliano que especifica a visibilidade de um título do eixo.|

## <a name="relationships"></a>Relacionamentos
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|formato|[ChartAxisTitleFormat](chartaxistitleformat.md)|Representa a formatação do título do eixo do gráfico. Somente leitura.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chartAxisTitle"
}-->

```json
{
  "text": "string",
  "visible": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartAxisTitle resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
