---
title: Tipo de recurso sizeRange
description: Especifica os tamanhos mínimo e máximo (em kilobytes) que uma mensagem de entrada deve ter para que a condição ou exceção seja aplicada.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: db90f040eef98af1136be7a80323dbedfe0acb92
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520510"
---
# <a name="sizerange-resource-type"></a>Tipo de recurso sizeRange

Namespace: Microsoft. Graph

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
