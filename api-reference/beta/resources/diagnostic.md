---
title: tipo de recurso de diagnóstico
description: Informações sobre um erro ou aviso para uma operação do OneNote.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: f0d5e6a938c454ca2efeda0dd7628c15269d6311
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507237"
---
# <a name="diagnostic-resource-type"></a>tipo de recurso de diagnóstico

Namespace: Microsoft. Graph

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
