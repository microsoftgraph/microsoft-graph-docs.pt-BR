---
title: tipo de recurso applicationEnforcedRestrictionsSessionControl
description: Controle de sessão para impor restrições de aplicativo.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: b5f608a2915db80d671ab604ab69d256d6aad0ec
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508286"
---
# <a name="applicationenforcedrestrictionssessioncontrol-resource-type"></a>tipo de recurso applicationEnforcedRestrictionsSessionControl

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Controle de sessão para impor restrições de aplicativo. Inehrits do [controle de sessão de acesso condicional](conditionalaccesssessioncontrol.md).

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|isEnabled     |Boolean      | Especifica se o controle de sessão está habilitado ou não. |

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.applicationEnforcedRestrictionsSessionControl",
  "baseType": "microsoft.graph.conditionalAccessSessionControl"
}-->

```json
{
  "isEnabled": true
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "applicationEnforcedRestrictionsSessionControl resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
