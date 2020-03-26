---
title: tipo de recurso callRoute
description: Representa o tipo de rota de chamada.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: d316c6ba9a7a9d34b34110023019169c39859c79
ms.sourcegitcommit: 115890bc7e7a54db8a2befeb8f720a9ca94f42b5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/26/2020
ms.locfileid: "42962516"
---
# <a name="callroute-resource-type"></a><span data-ttu-id="2590b-103">tipo de recurso callRoute</span><span class="sxs-lookup"><span data-stu-id="2590b-103">callRoute resource type</span></span>

<span data-ttu-id="2590b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2590b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2590b-105">Representa o tipo de rota de chamada.</span><span class="sxs-lookup"><span data-stu-id="2590b-105">Represents the call route type.</span></span>

## <a name="properties"></a><span data-ttu-id="2590b-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2590b-106">Properties</span></span>

| <span data-ttu-id="2590b-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2590b-107">Property</span></span>            | <span data-ttu-id="2590b-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="2590b-108">Type</span></span>                          | <span data-ttu-id="2590b-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="2590b-109">Description</span></span>                                                  |
| :------------------ | :---------------------------- | :----------------------------------------------------------- |
| <span data-ttu-id="2590b-110">recente</span><span class="sxs-lookup"><span data-stu-id="2590b-110">final</span></span>               | [<span data-ttu-id="2590b-111">identitySet</span><span class="sxs-lookup"><span data-stu-id="2590b-111">identitySet</span></span>](identityset.md) | <span data-ttu-id="2590b-112">A identidade que foi resolvida para na chamada.</span><span class="sxs-lookup"><span data-stu-id="2590b-112">The identity that was resolved to in the call.</span></span>               |
| <span data-ttu-id="2590b-113">Original</span><span class="sxs-lookup"><span data-stu-id="2590b-113">original</span></span>            | [<span data-ttu-id="2590b-114">identitySet</span><span class="sxs-lookup"><span data-stu-id="2590b-114">identitySet</span></span>](identityset.md) | <span data-ttu-id="2590b-115">A identidade que foi usada originalmente na chamada.</span><span class="sxs-lookup"><span data-stu-id="2590b-115">The identity that was originally used in the call.</span></span>           |
| <span data-ttu-id="2590b-116">RoutingType</span><span class="sxs-lookup"><span data-stu-id="2590b-116">routingType</span></span>         | <span data-ttu-id="2590b-117">String</span><span class="sxs-lookup"><span data-stu-id="2590b-117">String</span></span>                        | <span data-ttu-id="2590b-118">Os valores possíveis são: `forwarded`, `lookup`, `selfFork`.</span><span class="sxs-lookup"><span data-stu-id="2590b-118">Possible values are: `forwarded`, `lookup`, `selfFork`.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="2590b-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2590b-119">JSON representation</span></span>

<span data-ttu-id="2590b-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2590b-120">The following is a JSON representation of the resource.</span></span>

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
