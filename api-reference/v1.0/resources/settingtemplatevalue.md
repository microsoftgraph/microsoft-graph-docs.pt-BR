---
title: configuraçãoSplateValue tipo de recurso
description: Representa uma definição de configuração de modelo individual, incluindo o valor padrão da configuração, se a configuração não for instantânea.
localization_priority: Normal
author: dkershaw10
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: e53a8f07f325b023deea32e01fe217feeb35f49d
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2021
ms.locfileid: "52547047"
---
# <a name="settingtemplatevalue-resource-type"></a>configuraçãoSplateValue tipo de recurso

Namespace: microsoft.graph

Representa uma definição de configuração de modelo individual, incluindo o valor padrão da configuração, se a configuração não for instantânea.

### <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:---------------|:--------|:----------|
|defaultValue|Cadeia de caracteres| Valor padrão para a configuração. |
|descrição|Cadeia de caracteres| Descrição da configuração. |
|nome|Cadeia de caracteres| Nome da configuração. |
|tipo|Cadeia de caracteres| Tipo de configuração. |

### <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.settingTemplateValue"
}-->

```json
{
  "defaultValue": "String",
  "description": "String",
  "name": "String",
  "type": "String"
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "settingTemplateValue resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

