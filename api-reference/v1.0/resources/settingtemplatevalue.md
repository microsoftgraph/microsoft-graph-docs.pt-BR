---
title: tipo de recurso settingTemplateValue
description: Representa uma definição de configuração de modelo individual, incluindo o valor padrão para a configuração, se a configuração não for instautada.
ms.localizationpriority: medium
author: dkershaw10
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 307161ccb879985942f0973b29fc4cbc370c230c
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59126650"
---
# <a name="settingtemplatevalue-resource-type"></a>tipo de recurso settingTemplateValue

Namespace: microsoft.graph

Representa uma definição de configuração de modelo individual, incluindo o valor padrão para a configuração, se a configuração não for instautada.

### <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:---------------|:--------|:----------|
|defaultValue|String| Valor padrão para a configuração. |
|description|Cadeia de caracteres| Descrição da configuração. |
|nome|String| Nome da configuração. |
|tipo|Cadeia de caracteres| Tipo da configuração. |

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

