---
title: Tipo de recurso sizeRange
description: Especifica os tamanhos mínimo e máximo (em kilobytes) que uma mensagem de entrada deve ter para que a condição ou exceção seja aplicada.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 68fb44ff091720520c5061f0421d3819a8eed176
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965002"
---
# <a name="sizerange-resource-type"></a>Tipo de recurso sizeRange

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Especifica os tamanhos mínimo e máximo (em kilobytes) que uma mensagem de entrada deve ter para que a condição ou exceção seja aplicada.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
| maximumSize | Int32 | Especifica o tamanho máximo (em kilobytes) que uma mensagem de entrada deve ter para que a condição ou exceção seja aplicada. |
| minimumSize | Int32 | Especifica o tamanho mínimo (em kilobytes) que uma mensagem de entrada deve ter para que a condição ou exceção seja aplicada. |


## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
   ],
  "@odata.type": "microsoft.graph.sizeRange"
}-->

```json
{
  "maximumSize": "Int32",
  "minimumSize": "Int32"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "sizeRange resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
