---
title: tipo de recurso fallbackPolicy
description: 'Permite que a política de fallback seja especificada somente para os pontos de extremidade iOS e tenha sido projetada para ser usada para notificações brutas de alta prioridade. '
localization_priority: Normal
author: merzink
ms.prod: notifications
doc_type: resourcePageType
ms.openlocfilehash: d9f3f545c8566d4fe363e4dfabaa41f382a96a59
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938966"
---
# <a name="fallbackpolicy-resource-type"></a><span data-ttu-id="aa716-103">tipo de recurso fallbackPolicy</span><span class="sxs-lookup"><span data-stu-id="aa716-103">fallbackPolicy resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aa716-104">Permite que a política de fallback seja especificada somente para os pontos de extremidade iOS, e foi projetada para ser usada para notificações brutas de alta prioridade que podem não ser entregues aos dispositivos devido a restrições específicas de plataforma (por exemplo, modo economia de bateria).</span><span class="sxs-lookup"><span data-stu-id="aa716-104">Allows fallback policy to be specified for iOS endpoints only and is designed to be used for high-priority raw notifications that might not be delivered to devices due to platform specific restrictions (e.g. battery saver mode).</span></span>

## <a name="properties"></a><span data-ttu-id="aa716-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="aa716-105">Properties</span></span>

| <span data-ttu-id="aa716-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="aa716-106">Property</span></span>     | <span data-ttu-id="aa716-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="aa716-107">Type</span></span>        | <span data-ttu-id="aa716-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="aa716-108">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="aa716-109">endpointFallback</span><span class="sxs-lookup"><span data-stu-id="aa716-109">endpointFallback</span></span> | [<span data-ttu-id="aa716-110">fallbackPolicyProperties</span><span class="sxs-lookup"><span data-stu-id="aa716-110">fallbackPolicyProperties</span></span>](fallbackpolicyproperties.md) | <span data-ttu-id="aa716-111">O objeto de política EndpointFallback manipula a política de fallback de notificação em um nível de ponto final e está limitado ao iOS.</span><span class="sxs-lookup"><span data-stu-id="aa716-111">EndpointFallback policy object handles notification fallback policy at an end point level and is currently limited to iOS.</span></span> |   


## <a name="json-representation"></a><span data-ttu-id="aa716-112">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="aa716-112">JSON representation</span></span>

<span data-ttu-id="aa716-113">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="aa716-113">The following is a JSON representation of the resource.</span></span>

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
