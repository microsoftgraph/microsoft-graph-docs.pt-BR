---
title: tipo de recurso de modifiedProperty
description: Indica a todas as propriedades modificadas com valor antigo e o novo valor para qualquer recurso no Azure AD que foi alterado
ms.openlocfilehash: c504969ee12798969aa39490e79cb5b60bdb5435
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27035767"
---
# <a name="modifiedproperty-resource-type"></a>tipo de recurso de modifiedProperty
Indica a todas as propriedades modificadas com valor antigo e o novo valor para qualquer recurso no Azure AD que foi alterado



## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|displayName|String|Indica o nome da propriedade do atributo-alvo que foi alterado.|
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