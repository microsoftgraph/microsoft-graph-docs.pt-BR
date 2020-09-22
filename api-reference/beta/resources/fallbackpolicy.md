---
title: tipo de recurso fallbackPolicy
description: 'Permite que a política de fallback seja especificada somente para os pontos de extremidade iOS e tenha sido projetada para ser usada para notificações brutas de alta prioridade. '
localization_priority: Normal
author: merzink
ms.prod: notifications
doc_type: resourcePageType
ms.openlocfilehash: 8d39f9b69eb4ebdfcab883adec10b70100efba4f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48071207"
---
# <a name="fallbackpolicy-resource-type"></a><span data-ttu-id="1b965-103">tipo de recurso fallbackPolicy</span><span class="sxs-lookup"><span data-stu-id="1b965-103">fallbackPolicy resource type</span></span>

<span data-ttu-id="1b965-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1b965-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1b965-105">Permite que a política de fallback seja especificada somente para os pontos de extremidade iOS, e foi projetada para ser usada para notificações brutas de alta prioridade que podem não ser entregues aos dispositivos devido a restrições específicas de plataforma (por exemplo, modo economia de bateria).</span><span class="sxs-lookup"><span data-stu-id="1b965-105">Allows fallback policy to be specified for iOS endpoints only and is designed to be used for high-priority raw notifications that might not be delivered to devices due to platform specific restrictions (e.g. battery saver mode).</span></span>

## <a name="properties"></a><span data-ttu-id="1b965-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1b965-106">Properties</span></span>

| <span data-ttu-id="1b965-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1b965-107">Property</span></span>     | <span data-ttu-id="1b965-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="1b965-108">Type</span></span>        | <span data-ttu-id="1b965-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="1b965-109">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="1b965-110">endpointFallback</span><span class="sxs-lookup"><span data-stu-id="1b965-110">endpointFallback</span></span> | [<span data-ttu-id="1b965-111">fallbackpolicyProperties</span><span class="sxs-lookup"><span data-stu-id="1b965-111">fallbackpolicyProperties</span></span>](fallbackpolicyproperties.md) | <span data-ttu-id="1b965-112">O objeto de política EndpointFallback manipula a política de fallback de notificação em um nível de ponto final e está limitado ao iOS.</span><span class="sxs-lookup"><span data-stu-id="1b965-112">EndpointFallback policy object handles notification fallback policy at an end point level and is currently limited to iOS.</span></span> |   


## <a name="json-representation"></a><span data-ttu-id="1b965-113">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1b965-113">JSON representation</span></span>

<span data-ttu-id="1b965-114">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1b965-114">The following is a JSON representation of the resource.</span></span>

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


