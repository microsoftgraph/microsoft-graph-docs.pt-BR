---
title: tipo de recurso callRoute
description: O tipo callRoute.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 698cf2d6c2ae8b157aee4db45219eeb0b85c73c5
ms.sourcegitcommit: 9bddc0b7746383e8d05ce50d163af3f4196f12a6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/06/2019
ms.locfileid: "38006737"
---
# <a name="callroute-resource-type"></a><span data-ttu-id="38a8a-103">tipo de recurso callRoute</span><span class="sxs-lookup"><span data-stu-id="38a8a-103">callRoute resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="38a8a-104">O tipo callRoute.</span><span class="sxs-lookup"><span data-stu-id="38a8a-104">The callRoute type.</span></span>

## <a name="properties"></a><span data-ttu-id="38a8a-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="38a8a-105">Properties</span></span>

| <span data-ttu-id="38a8a-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="38a8a-106">Property</span></span>            | <span data-ttu-id="38a8a-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="38a8a-107">Type</span></span>                          | <span data-ttu-id="38a8a-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="38a8a-108">Description</span></span>                                                  |
| :------------------ | :---------------------------- | :----------------------------------------------------------- |
| <span data-ttu-id="38a8a-109">recente</span><span class="sxs-lookup"><span data-stu-id="38a8a-109">final</span></span>               | [<span data-ttu-id="38a8a-110">identitySet</span><span class="sxs-lookup"><span data-stu-id="38a8a-110">identitySet</span></span>](identityset.md) | <span data-ttu-id="38a8a-111">A identidade que foi resolvida para na chamada.</span><span class="sxs-lookup"><span data-stu-id="38a8a-111">The identity that was resolved to in the call.</span></span>               |
| <span data-ttu-id="38a8a-112">Original</span><span class="sxs-lookup"><span data-stu-id="38a8a-112">original</span></span>            | [<span data-ttu-id="38a8a-113">identitySet</span><span class="sxs-lookup"><span data-stu-id="38a8a-113">identitySet</span></span>](identityset.md) | <span data-ttu-id="38a8a-114">A identidade que foi usada originalmente na chamada.</span><span class="sxs-lookup"><span data-stu-id="38a8a-114">The identity that was originally used in the call.</span></span>           |
| <span data-ttu-id="38a8a-115">RoutingType</span><span class="sxs-lookup"><span data-stu-id="38a8a-115">routingType</span></span>         | <span data-ttu-id="38a8a-116">String</span><span class="sxs-lookup"><span data-stu-id="38a8a-116">String</span></span>                        | <span data-ttu-id="38a8a-117">Os valores possíveis são: `forwarded`, `lookup`, `selfFork`.</span><span class="sxs-lookup"><span data-stu-id="38a8a-117">Possible values are: `forwarded`, `lookup`, `selfFork`.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="38a8a-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="38a8a-118">JSON representation</span></span>

<span data-ttu-id="38a8a-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="38a8a-119">The following is a JSON representation of the resource.</span></span>

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
