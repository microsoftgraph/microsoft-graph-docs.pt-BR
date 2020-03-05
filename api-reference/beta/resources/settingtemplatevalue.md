---
title: tipo de recurso settingTemplateValue
description: Representa uma definição de configuração de modelo individual, incluindo o valor padrão para a configuração, se a configuração não for instanciada.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: cbd53a704e37b6f0cfa15cc875d5de000627b76c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520756"
---
# <a name="settingtemplatevalue-resource-type"></a>tipo de recurso settingTemplateValue

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma definição de configuração de modelo individual, incluindo o valor padrão para a configuração, se a configuração não for instanciada.


## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|defaultValue|string|Valor padrão para a configuração. Somente leitura.|
|description|string|Descrição da configuração. Somente leitura.|
|name|cadeia de caracteres|Nome da configuração. Somente leitura.|
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
