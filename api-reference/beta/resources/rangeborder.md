---
title: Tipo de recurso RangeBorder
description: Representa a borda de um objeto.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 33ed0410ab807cf9d9d6a0a49cb06b43d9966e46
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27853526"
---
# <a name="rangeborder-resource-type"></a>Tipo de recurso RangeBorder

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Representa a borda de um objeto.


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Get RangeBorder](../api/rangeborder-get.md) | [RangeBorder](rangeborder.md) |Leia as propriedades e relacionamentos do objeto rangeBorder.|
|[Update](../api/rangeborder-update.md) | [RangeBorder](rangeborder.md) |Atualize o objeto RangeBorder. |
|[List](../api/rangeborder-list.md) | Coleção [RangeBorder](rangeborder.md) |Obtenha a coleção de objetos rangeBorder. |
|[Itemat](../api/rangebordercollection-itemat.md)|[RangeBorder](rangeborder.md)|Obtém um objeto de borda usando seu índice.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|color|string|Código de cor HTML que representa a cor #RRGGBB da linha de borda do formulário (por exemplo, "FFA500") ou uma cor HTML nomeada (por exemplo, "laranja").|
|id|string|Representa o identificador da borda. Os valores possíveis são: `EdgeTop`, `EdgeBottom`, `EdgeLeft`, `EdgeRight`, `InsideVertical`, `InsideHorizontal`, `DiagonalDown` e `DiagonalUp`. Somente leitura.|
|sideIndex|string|Valor constante que indica o lado específico da borda. Os valores possíveis são: `EdgeTop`, `EdgeBottom`, `EdgeLeft`, `EdgeRight`, `InsideVertical`, `InsideHorizontal`, `DiagonalDown` e `DiagonalUp`. Somente leitura.|
|style|string|Uma das constantes de estilo de linha especificando o estilo de linha da borda. Os valores possíveis são: `None`, `Continuous`, `Dash`, `DashDot`, `DashDotDot`, `Dot`, `Double` e `SlantDashDot`.|
|weight|string|Especifica a espessura da borda em torno de um intervalo. Os valores possíveis são: `Hairline`, `Thin`, `Medium` e `Thick`.|

## <a name="relationships"></a>Relações
Nenhum


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.rangeBorder"
}-->

```json
{
  "color": "string",
  "id": "string",
  "sideIndex": "string",
  "style": "string",
  "weight": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "RangeBorder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
