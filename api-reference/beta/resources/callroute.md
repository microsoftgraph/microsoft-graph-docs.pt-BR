---
title: tipo de recurso callRoute
description: O tipo callRoute.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 9978bffd55f62f0646f84d2405df70eba6232d68
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35974050"
---
# <a name="callroute-resource-type"></a><span data-ttu-id="10e27-103">tipo de recurso callRoute</span><span class="sxs-lookup"><span data-stu-id="10e27-103">callRoute resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="10e27-104">O tipo callRoute.</span><span class="sxs-lookup"><span data-stu-id="10e27-104">The callRoute type.</span></span>

## <a name="properties"></a><span data-ttu-id="10e27-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="10e27-105">Properties</span></span>

| <span data-ttu-id="10e27-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="10e27-106">Property</span></span>            | <span data-ttu-id="10e27-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="10e27-107">Type</span></span>                          | <span data-ttu-id="10e27-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="10e27-108">Description</span></span>                                                  |
| :------------------ | :---------------------------- | :----------------------------------------------------------- |
| <span data-ttu-id="10e27-109">recente</span><span class="sxs-lookup"><span data-stu-id="10e27-109">final</span></span>               | [<span data-ttu-id="10e27-110">identitySet</span><span class="sxs-lookup"><span data-stu-id="10e27-110">identitySet</span></span>](identityset.md) | <span data-ttu-id="10e27-111">A identidade que foi resolvida para na chamada.</span><span class="sxs-lookup"><span data-stu-id="10e27-111">The identity that was resolved to in the call.</span></span>               |
| <span data-ttu-id="10e27-112">Original</span><span class="sxs-lookup"><span data-stu-id="10e27-112">original</span></span>            | [<span data-ttu-id="10e27-113">identitySet</span><span class="sxs-lookup"><span data-stu-id="10e27-113">identitySet</span></span>](identityset.md) | <span data-ttu-id="10e27-114">A identidade que foi usada originalmente na chamada.</span><span class="sxs-lookup"><span data-stu-id="10e27-114">The identity that was originally used in the call.</span></span>           |
| <span data-ttu-id="10e27-115">RoutingType</span><span class="sxs-lookup"><span data-stu-id="10e27-115">routingType</span></span>         | <span data-ttu-id="10e27-116">String</span><span class="sxs-lookup"><span data-stu-id="10e27-116">String</span></span>                        | <span data-ttu-id="10e27-117">Os valores possíveis são: `forwarded`, `lookup`, `selfFork`.</span><span class="sxs-lookup"><span data-stu-id="10e27-117">Possible values are: `forwarded`, `lookup`, `selfFork`.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="10e27-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="10e27-118">JSON representation</span></span>

<span data-ttu-id="10e27-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="10e27-119">The following is a JSON representation of the resource.</span></span>

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
