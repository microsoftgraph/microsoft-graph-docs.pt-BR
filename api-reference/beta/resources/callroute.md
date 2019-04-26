---
title: tipo de recurso callRoute
description: O tipo callRoute.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 06dd1a2265c5a6bda9feba0b51e7fd731d7945c3
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33328273"
---
# <a name="callroute-resource-type"></a><span data-ttu-id="95a5f-103">tipo de recurso callRoute</span><span class="sxs-lookup"><span data-stu-id="95a5f-103">callRoute resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="95a5f-104">O tipo callRoute.</span><span class="sxs-lookup"><span data-stu-id="95a5f-104">The callRoute type.</span></span>

## <a name="properties"></a><span data-ttu-id="95a5f-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="95a5f-105">Properties</span></span>

| <span data-ttu-id="95a5f-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="95a5f-106">Property</span></span>            | <span data-ttu-id="95a5f-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="95a5f-107">Type</span></span>                          | <span data-ttu-id="95a5f-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="95a5f-108">Description</span></span>                                                  |
| :------------------ | :---------------------------- | :----------------------------------------------------------- |
| <span data-ttu-id="95a5f-109">recente</span><span class="sxs-lookup"><span data-stu-id="95a5f-109">final</span></span>               | [<span data-ttu-id="95a5f-110">identitySet</span><span class="sxs-lookup"><span data-stu-id="95a5f-110">identitySet</span></span>](identityset.md) | <span data-ttu-id="95a5f-111">A identidade que foi resolvida para na chamada.</span><span class="sxs-lookup"><span data-stu-id="95a5f-111">The identity that was resolved to in the call.</span></span>               |
| <span data-ttu-id="95a5f-112">Original</span><span class="sxs-lookup"><span data-stu-id="95a5f-112">original</span></span>            | [<span data-ttu-id="95a5f-113">identitySet</span><span class="sxs-lookup"><span data-stu-id="95a5f-113">identitySet</span></span>](identityset.md) | <span data-ttu-id="95a5f-114">A identidade que foi usada originalmente na chamada.</span><span class="sxs-lookup"><span data-stu-id="95a5f-114">The identity that was originally used in the call.</span></span>           |
| <span data-ttu-id="95a5f-115">RoutingType</span><span class="sxs-lookup"><span data-stu-id="95a5f-115">routingType</span></span>         | <span data-ttu-id="95a5f-116">String</span><span class="sxs-lookup"><span data-stu-id="95a5f-116">String</span></span>                        | <span data-ttu-id="95a5f-117">Os valores possíveis são: `forwarded`, `lookup`, `selfFork`.</span><span class="sxs-lookup"><span data-stu-id="95a5f-117">Possible values are: `forwarded`, `lookup`, `selfFork`.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="95a5f-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="95a5f-118">JSON representation</span></span>

<span data-ttu-id="95a5f-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="95a5f-119">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.callRoute"
}-->
```json
{
  "final": {"@odata.type": "#microsoft.graph.identitySet"},
  "original": {"@odata.type": "#microsoft.graph.identitySet"},
  "routingType": "forwarded | lookup | selfFork"
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "callRoute resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
