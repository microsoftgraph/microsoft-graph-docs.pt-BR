---
title: Tipo de recurso applicationEnforcedRestrictionsSessionControl
description: Controle de sessão para impor restrições de aplicativo.
localization_priority: Normal
author: sureshja
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: f7f20950b3773e660cfc1b0ed4fdec338546e09a
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50134762"
---
# <a name="applicationenforcedrestrictionssessioncontrol-resource-type"></a>Tipo de recurso applicationEnforcedRestrictionsSessionControl

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Controle de sessão para impor restrições de aplicativo. Inehrits do [Controle de Sessão de Acesso Condicional.](conditionalaccesssessioncontrol.md)

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|isEnabled     |Booliano      | Especifica se o controle de sessão está habilitado ou não. |

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


