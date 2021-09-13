---
title: tipo de recurso settingValue
description: Uma configuração representada por um par de nomes/valores.
ms.localizationpriority: medium
author: dkershaw10
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: 93d7fbfca62f4d34b3a2640c5ae6eb7e91c59a1a
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59126643"
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

