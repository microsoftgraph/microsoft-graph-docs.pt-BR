---
title: Tipo de recurso settingValue
description: Uma configuração representada por um par nome/valor.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: directory-management
author: dkershaw10
ms.openlocfilehash: d1be40f6ad2046895c1a14f3395185662ae0ff62
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133375"
---
# <a name="settingvalue-resource-type"></a>Tipo de recurso settingValue

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Uma configuração representada por um par nome/valor.


## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|nome|string|Nome da configuração (conforme definido pelo directorySettingTemplate).|
|value|string|Valor da configuração.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.settingValue"
}-->

```json
{
  "name": "string",
  "value": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "settingValue resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


