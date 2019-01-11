---
title: Tipo de recurso extension
description: Um tipo abstrato para oferecer suporte ao tipo openTypeExtension livre do OData v4.
localization_priority: Normal
ms.openlocfilehash: 2633c8a28c1be1a670a80834ce869b5156fc1de9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27834668"
---
# <a name="extension-resource-type"></a>Tipo de recurso extension

Um tipo abstrato para oferecer suporte ao tipo [openTypeExtension](opentypeextension.md) livre do OData v4.

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!-- {
  "abstract": "true",
  "baseType": "microsoft.graph.entity",
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.extension"
}-->

```json
{
  "id": "string (identifier)"
}

```
## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|id|Cadeia de caracteres| Somente leitura.|

## <a name="relationships"></a>Relações
Nenhum


## <a name="methods"></a>Métodos

Consulte os métodos do tipo derivado [openTypeExtension](opentypeextension.md) para métodos que são realmente compatíveis.


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "extension resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
