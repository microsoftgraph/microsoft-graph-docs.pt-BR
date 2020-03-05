---
title: tipo de recurso SettingValue
description: Uma configuração representada por um par de nome/valor.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: ba9b6321ad443d9538d9c539435c62f50149b330
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42446888"
---
# <a name="settingvalue-resource-type"></a>tipo de recurso SettingValue

Namespace: Microsoft. Graph

Uma configuração representada por um par de nome/valor.

### <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:---------------|:--------|:----------|
|nome|String| Nome da configuração (conforme definido pelo [groupSettingTemplate](groupsettingtemplate.md)). |
|value|Cadeia de caracteres| Valor da configuração. |

### <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.settingValue"
}-->

```json
{
  "name": "String",
  "value": "String"
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "settingValue resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
