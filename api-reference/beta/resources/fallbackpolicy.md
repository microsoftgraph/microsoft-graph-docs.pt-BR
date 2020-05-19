---
title: tipo de recurso fallbackPolicy
description: 'Permite que a política de fallback seja especificada somente para os pontos de extremidade iOS e tenha sido projetada para ser usada para notificações brutas de alta prioridade. '
localization_priority: Normal
author: merzink
ms.prod: notifications
doc_type: resourcePageType
ms.openlocfilehash: 5fd76d6798ab92fdfa319b732dd926fbec22e798
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2020
ms.locfileid: "44290178"
---
# <a name="fallbackpolicy-resource-type"></a>tipo de recurso fallbackPolicy

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Permite que a política de fallback seja especificada somente para os pontos de extremidade iOS, e foi projetada para ser usada para notificações brutas de alta prioridade que podem não ser entregues aos dispositivos devido a restrições específicas de plataforma (por exemplo, modo economia de bateria).

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
| endpointFallback | [fallbackpolicyProperties](fallbackpolicyproperties.md) | O objeto de política EndpointFallback manipula a política de fallback de notificação em um nível de ponto final e está limitado ao iOS. |   


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.fallbackpolicy",
  "baseType": null
}-->

```json
{
  "endpointFallback": {"@odata.type": "microsoft.graph.fallbackpolicyProperties"}
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "fallbackpolicy resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
