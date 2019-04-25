---
title: tipo de recurso callRoute
description: O tipo callRoute.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: cfa470c4d3a03655221cab1f29baa60d00a8cf6c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543828"
---
# <a name="callroute-resource-type"></a><span data-ttu-id="b40be-103">tipo de recurso callRoute</span><span class="sxs-lookup"><span data-stu-id="b40be-103">callRoute resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b40be-104">O tipo callRoute.</span><span class="sxs-lookup"><span data-stu-id="b40be-104">The callRoute type.</span></span>

## <a name="properties"></a><span data-ttu-id="b40be-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b40be-105">Properties</span></span>

| <span data-ttu-id="b40be-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b40be-106">Property</span></span>            | <span data-ttu-id="b40be-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="b40be-107">Type</span></span>                          | <span data-ttu-id="b40be-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="b40be-108">Description</span></span>                                                  |
| :------------------ | :---------------------------- | :----------------------------------------------------------- |
| <span data-ttu-id="b40be-109">recente</span><span class="sxs-lookup"><span data-stu-id="b40be-109">final</span></span>               | [<span data-ttu-id="b40be-110">identitySet</span><span class="sxs-lookup"><span data-stu-id="b40be-110">identitySet</span></span>](identityset.md) | <span data-ttu-id="b40be-111">A identidade que foi resolvida para na chamada.</span><span class="sxs-lookup"><span data-stu-id="b40be-111">The identity that was resolved to in the call.</span></span>               |
| <span data-ttu-id="b40be-112">Original</span><span class="sxs-lookup"><span data-stu-id="b40be-112">original</span></span>            | [<span data-ttu-id="b40be-113">identitySet</span><span class="sxs-lookup"><span data-stu-id="b40be-113">identitySet</span></span>](identityset.md) | <span data-ttu-id="b40be-114">A identidade que foi usada originalmente na chamada.</span><span class="sxs-lookup"><span data-stu-id="b40be-114">The identity that was originally used in the call.</span></span>           |
| <span data-ttu-id="b40be-115">RoutingType</span><span class="sxs-lookup"><span data-stu-id="b40be-115">routingType</span></span>         | <span data-ttu-id="b40be-116">String</span><span class="sxs-lookup"><span data-stu-id="b40be-116">String</span></span>                        | <span data-ttu-id="b40be-117">Os valores possíveis são: `forwarded`, `lookup`, `selfFork`.</span><span class="sxs-lookup"><span data-stu-id="b40be-117">Possible values are: `forwarded`, `lookup`, `selfFork`.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="b40be-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b40be-118">JSON representation</span></span>

<span data-ttu-id="b40be-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b40be-119">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/callroute.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
