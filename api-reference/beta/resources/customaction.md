---
title: tipo de recurso customAction
description: Representa qualquer ação personalizada que um rótulo pode fornecer, se configurada pelo administrador.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: e2a660659f8c0f3a2c6dc571e743884c54365a20
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507321"
---
# <a name="customaction-resource-type"></a>tipo de recurso customAction

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa qualquer ação personalizada que um rótulo pode fornecer, se configurada pelo administrador. As ações personalizadas podem ser definidas como parte de um [informationProtectionLabel](informationProtectionLabel.md) por meio do módulo PowerShell do centro de conformidade e segurança do Office 365. As ações devem ser compreendidas pelo aplicativo de consumo.

## <a name="properties"></a>Propriedades

| Propriedade   | Tipo                                       | Descrição                                          |
| :--------- | :----------------------------------------- | :--------------------------------------------------- |
| nome       | String                                     | Nome da ação personalizada.                           |
| properties | Coleção [keyValuePair](keyvaluepair.md) | Propriedades, no formato par de valores chave, da ação. |

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