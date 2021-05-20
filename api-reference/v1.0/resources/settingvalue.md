---
title: configuraçãoEvase tipo de
description: Uma configuração representada por um par de nome/valor.
localization_priority: Normal
author: dkershaw10
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: 171b08d4542af6900dcb6549527e956c4395c947
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2021
ms.locfileid: "52547040"
---
# <a name="settingvalue-resource-type"></a>configuraçãoEvase tipo de

Namespace: microsoft.graph

Uma configuração representada por um par de nome/valor.

### <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:---------------|:--------|:----------|
|nome|Cadeia de caracteres| Nome da configuração (definida pelo [grupoSettingTemplate](groupsettingtemplate.md)). |
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

