---
title: tipo de recurso callRoute
description: O tipo callRoute.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 49ef6190f65adde817f3912d4133ff4a8553a88f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48027210"
---
# <a name="callroute-resource-type"></a><span data-ttu-id="38636-103">tipo de recurso callRoute</span><span class="sxs-lookup"><span data-stu-id="38636-103">callRoute resource type</span></span>

<span data-ttu-id="38636-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="38636-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="38636-105">O tipo callRoute.</span><span class="sxs-lookup"><span data-stu-id="38636-105">The callRoute type.</span></span>

## <a name="properties"></a><span data-ttu-id="38636-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="38636-106">Properties</span></span>

| <span data-ttu-id="38636-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="38636-107">Property</span></span>            | <span data-ttu-id="38636-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="38636-108">Type</span></span>                          | <span data-ttu-id="38636-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="38636-109">Description</span></span>                                                  |
| :------------------ | :---------------------------- | :----------------------------------------------------------- |
| <span data-ttu-id="38636-110">recente</span><span class="sxs-lookup"><span data-stu-id="38636-110">final</span></span>               | [<span data-ttu-id="38636-111">identitySet</span><span class="sxs-lookup"><span data-stu-id="38636-111">identitySet</span></span>](identityset.md) | <span data-ttu-id="38636-112">A identidade que foi resolvida para na chamada.</span><span class="sxs-lookup"><span data-stu-id="38636-112">The identity that was resolved to in the call.</span></span>               |
| <span data-ttu-id="38636-113">Original</span><span class="sxs-lookup"><span data-stu-id="38636-113">original</span></span>            | [<span data-ttu-id="38636-114">identitySet</span><span class="sxs-lookup"><span data-stu-id="38636-114">identitySet</span></span>](identityset.md) | <span data-ttu-id="38636-115">A identidade que foi usada originalmente na chamada.</span><span class="sxs-lookup"><span data-stu-id="38636-115">The identity that was originally used in the call.</span></span>           |
| <span data-ttu-id="38636-116">RoutingType</span><span class="sxs-lookup"><span data-stu-id="38636-116">routingType</span></span>         | <span data-ttu-id="38636-117">String</span><span class="sxs-lookup"><span data-stu-id="38636-117">String</span></span>                        | <span data-ttu-id="38636-118">Os valores possíveis são: `forwarded`, `lookup`, `selfFork`.</span><span class="sxs-lookup"><span data-stu-id="38636-118">Possible values are: `forwarded`, `lookup`, `selfFork`.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="38636-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="38636-119">JSON representation</span></span>

<span data-ttu-id="38636-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="38636-120">The following is a JSON representation of the resource.</span></span>

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


