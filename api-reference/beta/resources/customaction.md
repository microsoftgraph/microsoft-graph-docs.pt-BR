---
title: Tipo de recurso customAction
description: Representa todas as ações personalizadas que um rótulo pode fornecer, se configurado pelo administrador.
localization_priority: Normal
author: tommoser
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 1d9c88715cba6fc8faede1419b3c8809c3ec3f54
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50941803"
---
# <a name="customaction-resource-type"></a>Tipo de recurso customAction

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa todas as ações personalizadas que um rótulo pode fornecer, se configurado pelo administrador. Ações personalizadas podem ser definidas como parte de [um informationProtectionLabel](informationProtectionLabel.md) por meio do módulo powerShell do Centro de Conformidade e Segurança do Office 365. As ações devem ser compreendidas pelo aplicativo de consumo.

## <a name="properties"></a>Propriedades

| Propriedade   | Tipo                                       | Descrição                                          |
| :--------- | :----------------------------------------- | :--------------------------------------------------- |
| nome       | Cadeia de caracteres                                     | Nome da ação personalizada.                           |
| properties | Coleção [keyValuePair](keyvaluepair.md) | Propriedades, no formato par de valores-chave, da ação. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.customAction",
  "baseType": "microsoft.graph.informationProtectionAction"
}-->

```json
{
  "name": "String",
  "properties": [{"@odata.type": "microsoft.graph.keyValuePair"}]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "customAction resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

