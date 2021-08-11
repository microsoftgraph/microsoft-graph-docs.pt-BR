---
title: tipo de recurso settingValue
description: Uma configuração representada por um par de nomes/valores.
localization_priority: Normal
author: dkershaw10
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: b2128c754c3ae30b0ffd0a4be142a1b361ababe049b09e2336e92b8fa3186a90
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54149643"
---
# <a name="settingvalue-resource-type"></a>tipo de recurso settingValue

Namespace: microsoft.graph

Uma configuração representada por um par de nomes/valores.

### <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:---------------|:--------|:----------|
|nome|Cadeia de caracteres| Nome da configuração (conforme definido pelo [groupSettingTemplate](groupsettingtemplate.md)). |
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

