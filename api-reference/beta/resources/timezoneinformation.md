---
title: Tipo de recurso timeZoneInformation
description: Representa um fuso horário. O formato com suporte é Windows e o fuso horário da autoridade de números atribuídos pela Internet (IANA) (também conhecido como fuso horário Olson)
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 3deae74f1ffc991e6e9178a46575c21d69272d2c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519677"
---
# <a name="timezoneinformation-resource-type"></a>Tipo de recurso timeZoneInformation

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um fuso horário. Entre os formatos de fuso horário válidos estão o do Windows e o da [Autoridade para Atribuição de Números na Internet (IANA)](https://www.iana.org/time-zones) (também conhecido como fuso horário de Olson), além de quando o atual problema conhecido foi corrigido.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|alias|string|Um identificador para o fuso horário.|
|displayName|cadeia de caracteres|Uma sequência de caracteres de exibição que representa o fuso horário.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.timeZoneInformation"
}-->

```json
{
  "alias": "string",
  "displayName": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "timeZoneInformation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
