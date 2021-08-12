---
title: Tipo de recurso RangeFont
description: Esse objeto representa os atributos de fonte de um objeto, como nome, tamanho, cor, dentre outros.
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 3754449b328f8b6d1217970b352cc11b28e998cf2e1b4f931c0f106eb97dc1ed
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54152262"
---
# <a name="rangefont-resource-type"></a>Tipo de recurso RangeFont

Namespace: microsoft.graph

Esse objeto representa os atributos de fonte de um objeto, como nome, tamanho, cor, dentre outros.


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Get RangeFont](../api/rangefont-get.md) | [WorkbookRangeFont](rangefont.md) |Leia as propriedades e os relacionamentos do objeto rangeFormat.|
|[Update](../api/rangefont-update.md) | [WorkbookRangeFont](rangefont.md)   |Atualize o objeto RangeFont. |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|bold|booliano|Representa o status da fonte em negrito.|
|color|cadeia de caracteres|Representação de código de cor HTML para a cor do texto. Por exemplo, #FF0000 representa vermelho.|
|italic|booliano|Representa o status da fonte em itálico.|
|nome|string|Nome da fonte (por exemplo, "Calibri")|
|size|Double|Font Size|
|underline|string|Tipo de sublinhado aplicado à fonte. Os valores possíveis são: `None`, `Single`, `Double`, `SingleAccountant`, `DoubleAccountant`.|

## <a name="relationships"></a>Relações
Nenhum


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookRangeFont"
}-->

```json
{
  "bold": true,
  "color": "string",
  "italic": true,
  "name": "string",
  "size": 1024,
  "underline": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "RangeFont resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

