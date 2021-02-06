---
title: Tipo de recurso settingTemplateValue
description: Representa uma definição de configuração de modelo individual, incluindo o valor padrão para a configuração, se a configuração não for instaliada.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: directory-management
author: dkershaw10
ms.openlocfilehash: 15110b88b62352476619501c50457a5bd1db5a89
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50131625"
---
# <a name="settingtemplatevalue-resource-type"></a>Tipo de recurso settingTemplateValue

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma definição de configuração de modelo individual, incluindo o valor padrão para a configuração, se a configuração não for instaliada.


## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|defaultValue|string|Valor padrão da configuração. Somente leitura.|
|description|string|Descrição da configuração. Somente leitura.|
|name|string|Nome da configuração. Somente leitura.|
|type|string|Tipo da configuração. Somente leitura.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.settingTemplateValue"
}-->

```json
{
  "defaultValue": "string",
  "description": "string",
  "name": "string",
  "type": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "settingTemplateValue resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


