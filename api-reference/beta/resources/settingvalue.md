---
title: tipo de recurso SettingValue
description: Uma configuração representada por um par de nome/valor.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: dkershaw10
ms.openlocfilehash: 1710bd136391a8c7d6d38217cb1635407570086f
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46806247"
---
# <a name="settingvalue-resource-type"></a>tipo de recurso SettingValue

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Uma configuração representada por um par de nome/valor.


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
