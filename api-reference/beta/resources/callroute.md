---
title: tipo de recurso callRoute
description: O tipo callRoute.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: bdc4c54f9f5676496ae64e97b1ce14e3918e7cc9
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/31/2019
ms.locfileid: "40913314"
---
# <a name="callroute-resource-type"></a><span data-ttu-id="e41e7-103">tipo de recurso callRoute</span><span class="sxs-lookup"><span data-stu-id="e41e7-103">callRoute resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e41e7-104">O tipo callRoute.</span><span class="sxs-lookup"><span data-stu-id="e41e7-104">The callRoute type.</span></span>

## <a name="properties"></a><span data-ttu-id="e41e7-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e41e7-105">Properties</span></span>

| <span data-ttu-id="e41e7-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e41e7-106">Property</span></span>            | <span data-ttu-id="e41e7-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="e41e7-107">Type</span></span>                          | <span data-ttu-id="e41e7-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="e41e7-108">Description</span></span>                                                  |
| :------------------ | :---------------------------- | :----------------------------------------------------------- |
| <span data-ttu-id="e41e7-109">recente</span><span class="sxs-lookup"><span data-stu-id="e41e7-109">final</span></span>               | [<span data-ttu-id="e41e7-110">identitySet</span><span class="sxs-lookup"><span data-stu-id="e41e7-110">identitySet</span></span>](identityset.md) | <span data-ttu-id="e41e7-111">A identidade que foi resolvida para na chamada.</span><span class="sxs-lookup"><span data-stu-id="e41e7-111">The identity that was resolved to in the call.</span></span>               |
| <span data-ttu-id="e41e7-112">Original</span><span class="sxs-lookup"><span data-stu-id="e41e7-112">original</span></span>            | [<span data-ttu-id="e41e7-113">identitySet</span><span class="sxs-lookup"><span data-stu-id="e41e7-113">identitySet</span></span>](identityset.md) | <span data-ttu-id="e41e7-114">A identidade que foi usada originalmente na chamada.</span><span class="sxs-lookup"><span data-stu-id="e41e7-114">The identity that was originally used in the call.</span></span>           |
| <span data-ttu-id="e41e7-115">RoutingType</span><span class="sxs-lookup"><span data-stu-id="e41e7-115">routingType</span></span>         | <span data-ttu-id="e41e7-116">String</span><span class="sxs-lookup"><span data-stu-id="e41e7-116">String</span></span>                        | <span data-ttu-id="e41e7-117">Os valores possíveis são: `forwarded`, `lookup`, `selfFork`.</span><span class="sxs-lookup"><span data-stu-id="e41e7-117">Possible values are: `forwarded`, `lookup`, `selfFork`.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="e41e7-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e41e7-118">JSON representation</span></span>

<span data-ttu-id="e41e7-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e41e7-119">The following is a JSON representation of the resource.</span></span>

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
