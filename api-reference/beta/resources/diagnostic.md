---
title: tipo de recurso de diagnóstico
description: Informações sobre um erro ou aviso para uma operação do OneNote.
localization_priority: Normal
ms.openlocfilehash: 63e146cd44e3e2866d9d632fb78cbc222443c9d8
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33340865"
---
# <a name="diagnostic-resource-type"></a>tipo de recurso de diagnóstico

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Informações sobre um erro ou aviso para uma operação do OneNote.

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.diagnostic"
}-->

```json
{
  "message": "string",
  "url": "string"
}

```
## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|mensagem|String|A mensagem que descreve a condição que disparou o erro ou aviso.|
|url|Cadeia de caracteres|O link para a documentação para esse problema.|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "diagnostic resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
