---
title: tipo de recurso de modifiedProperty
description: Indica a todas as propriedades modificadas com valor antigo e o novo valor para qualquer recurso no Azure AD que foi alterado
localization_priority: Normal
ms.openlocfilehash: 91e5df357a40b2e44bb26edc5fb3bf6965a260e5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27844448"
---
# <a name="modifiedproperty-resource-type"></a>tipo de recurso de modifiedProperty
Indica a todas as propriedades modificadas com valor antigo e o novo valor para qualquer recurso no Azure AD que foi alterado



## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|displayName|Cadeia de caracteres|Indica o nome da propriedade do atributo-alvo que foi alterado.|
|newValue|Cadeia de caracteres|Indica o valor atualizado para a propriedade.|
|oldValue|Cadeia de caracteres|Indica o valor anterior (antes da atualização) para a propriedade.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.modifiedProperty"
}-->

```json
{
  "displayName": "String",
  "newValue": "String",
  "oldValue": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "modifiedProperty resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
