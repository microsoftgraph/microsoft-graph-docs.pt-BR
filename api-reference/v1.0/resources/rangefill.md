---
title: Tipo de recurso RangeFill
description: Representa a tela de fundo de um objeto Range.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: c1485d3465818b9daccf039c13c21c7557206025886747110813e5b3834e6504
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54159852"
---
# <a name="rangefill-resource-type"></a>Tipo de recurso RangeFill

Namespace: microsoft.graph

Representa a tela de fundo de um objeto Range.


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Get RangeFill](../api/rangefill-get.md) | [WorkbookRangeFill](rangefill.md) |Leia as propriedades e os relacionamentos do objeto rangeFill.|
|[Update](../api/rangefill-update.md) | [WorkbookRangeFill](rangefill.md)   |Atualize o objeto RangeFill. |
|[Clear](../api/rangefill-clear.md)|Nenhum|Redefine o plano de fundo do intervalo.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|color|string|Código de cor HTML que representa a cor #RRGGBB da linha de borda do formulário (por exemplo, "FFA500") ou uma cor HTML nomeada (por exemplo, "laranja").|

## <a name="relationships"></a>Relações
Nenhum


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookRangeFill"
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
  "description": "RangeFill resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

