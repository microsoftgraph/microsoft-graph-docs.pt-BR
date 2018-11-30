---
title: Tipo de recurso ChartTitle
description: Representa um objeto de título de gráfico de um gráfico.
ms.openlocfilehash: ce2091c0cbd2435d96a1a931f7e46d6e2b8fb920
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27040700"
---
# <a name="charttitle-resource-type"></a>Tipo de recurso ChartTitle

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Representa um objeto de título de gráfico de um gráfico.


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Get ChartTitle](../api/charttitle-get.md) | [ChartTitle](charttitle.md) |Leia as propriedades e os relacionamentos do objeto chartTitle.|
|[Update](../api/charttitle-update.md) | [ChartTitle](charttitle.md)    |Atualize o objeto ChartTitle. |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|overlay|booliano|Valor booliano que determina se o título do gráfico deve se sobrepor ao gráfico ou não.|
|texto|string|Representa o texto do título de um gráfico.|
|visible|booliano|Um valor booliano que representa a visibilidade de um objeto de título de gráfico.|

## <a name="relationships"></a>Relacionamentos
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|formato|[ChartTitleFormat](charttitleformat.md)|Representa a formatação de um título do gráfico, que inclui a formatação de fonte e de preenchimento. Somente leitura.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chartTitle"
}-->

```json
{
  "overlay": true,
  "text": "string",
  "visible": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartTitle resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->