---
title: tipo de recurso workbookRangeFont
description: Esse objeto representa os atributos de fonte de um objeto, como nome, tamanho, cor, dentre outros.
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 9ddbb607a243f4571d53dcf887f80a171b230748
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519173"
---
# <a name="workbookrangefont-resource-type"></a>tipo de recurso workbookRangeFont

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Esse objeto representa os atributos de fonte de um objeto, como nome, tamanho, cor, dentre outros.


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Obter workbookRangeFont](../api/rangefont-get.md) | [workbookRangeFont](workbookrangefont.md) |Leia as propriedades e os relacionamentos do objeto rangeFormat.|
|[Update](../api/rangefont-update.md) | [workbookRangeFont](workbookrangefont.md)   |Atualize o objeto RangeFont. |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|bold|booliano|Representa o status da fonte em negrito.|
|color|cadeia de caracteres|Representação de código de cor HTML para a cor do texto. Por exemplo, #FF0000 representa vermelho.|
|italic|booliano|Representa o status da fonte em itálico.|
|nome|string|Nome da fonte (por exemplo, "Calibri")|
|size|Double|Font Size|
|underline| String |Tipo de sublinhado aplicado à fonte. Os valores possíveis são: `None`, `Single`, `Double`, `SingleAccountant` e `DoubleAccountant`.|

## <a name="relationships"></a>Relações
Nenhum


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
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
<!--
{
  "type": "#page.annotation",
  "description": "RangeFont resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
