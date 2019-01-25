---
title: Tipo de recurso locationConstraintItem
description: As condições indicadas por um cliente para o local de uma reunião.
localization_priority: Normal
ms.openlocfilehash: 9752b3acec2dd9071e31b743245d662168ecdfd6
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508850"
---
# <a name="locationconstraintitem-resource-type"></a><span data-ttu-id="3f0e3-103">Tipo de recurso locationConstraintItem</span><span class="sxs-lookup"><span data-stu-id="3f0e3-103">locationConstraintItem resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3f0e3-104">As condições indicadas por um cliente para o local de uma reunião.</span><span class="sxs-lookup"><span data-stu-id="3f0e3-104">The conditions stated by a client for the location of a meeting.</span></span>

<span data-ttu-id="3f0e3-105">Derivado de [location](location.md).</span><span class="sxs-lookup"><span data-stu-id="3f0e3-105">Derived from [location](location.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="3f0e3-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3f0e3-106">JSON representation</span></span>

<span data-ttu-id="3f0e3-107">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="3f0e3-107">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  
  ],
  "@odata.type": "microsoft.graph.locationConstraintItem"
}-->

```json
{
  "resolveAvailability": true,
  "address": {"@odata.type": "microsoft.graph.physicalAddress"},
  "coordinates": {"@odata.type": "microsoft.graph.outlookGeoCoordinates"},
  "displayName": "string",
  "locationEmailAddress": "string",
  "locationUri": "string"
}

```
## <a name="properties"></a><span data-ttu-id="3f0e3-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3f0e3-108">Properties</span></span>
| <span data-ttu-id="3f0e3-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3f0e3-109">Property</span></span>     | <span data-ttu-id="3f0e3-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="3f0e3-110">Type</span></span>   |<span data-ttu-id="3f0e3-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="3f0e3-111">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="3f0e3-112">address</span><span class="sxs-lookup"><span data-stu-id="3f0e3-112">address</span></span> | [<span data-ttu-id="3f0e3-113">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="3f0e3-113">physicalAddress</span></span>](physicaladdress.md) |<span data-ttu-id="3f0e3-114">O endereço físico do local.</span><span class="sxs-lookup"><span data-stu-id="3f0e3-114">The street address of the location.</span></span> |
| <span data-ttu-id="3f0e3-115">coordenadas</span><span class="sxs-lookup"><span data-stu-id="3f0e3-115">coordinates</span></span> | [<span data-ttu-id="3f0e3-116">outlookGeoCoordinates</span><span class="sxs-lookup"><span data-stu-id="3f0e3-116">outlookGeoCoordinates</span></span>](outlookgeocoordinates.md) | <span data-ttu-id="3f0e3-117">As coordenadas geográficas e a elevação do local.</span><span class="sxs-lookup"><span data-stu-id="3f0e3-117">The geographic coordinates and elevation of the location.</span></span> |
| <span data-ttu-id="3f0e3-118">displayName</span><span class="sxs-lookup"><span data-stu-id="3f0e3-118">displayName</span></span>  | <span data-ttu-id="3f0e3-119">String</span><span class="sxs-lookup"><span data-stu-id="3f0e3-119">String</span></span> | <span data-ttu-id="3f0e3-120">O nome associado ao local.</span><span class="sxs-lookup"><span data-stu-id="3f0e3-120">The name associated with the location.</span></span>                       |
| <span data-ttu-id="3f0e3-121">locationEmailAddress</span><span class="sxs-lookup"><span data-stu-id="3f0e3-121">locationEmailAddress</span></span> | <span data-ttu-id="3f0e3-122">String</span><span class="sxs-lookup"><span data-stu-id="3f0e3-122">String</span></span> | <span data-ttu-id="3f0e3-123">O endereço de email opcional do local.</span><span class="sxs-lookup"><span data-stu-id="3f0e3-123">Optional email address of the location.</span></span> |
| <span data-ttu-id="3f0e3-124">locationUri</span><span class="sxs-lookup"><span data-stu-id="3f0e3-124">locationUri</span></span> | <span data-ttu-id="3f0e3-125">String</span><span class="sxs-lookup"><span data-stu-id="3f0e3-125">String</span></span> | <span data-ttu-id="3f0e3-126">URI opcional que representa o local.</span><span class="sxs-lookup"><span data-stu-id="3f0e3-126">Optional URI representing the location.</span></span> |
| <span data-ttu-id="3f0e3-127">resolveAvailability</span><span class="sxs-lookup"><span data-stu-id="3f0e3-127">resolveAvailability</span></span> | <span data-ttu-id="3f0e3-128">Booliano</span><span class="sxs-lookup"><span data-stu-id="3f0e3-128">Boolean</span></span> | <span data-ttu-id="3f0e3-p101">Se definido como true e o recurso especificado está ocupado, [findMeetingTimes](../api/user-findmeetingtimes.md) procura outro recurso livre. Se definido como false e o recurso especificado está ocupado, **findMeetingTimes** retorna o recurso melhor classificado no cache do usuário sem verificar se ele está livre. O padrão é true.</span><span class="sxs-lookup"><span data-stu-id="3f0e3-p101">If set to true and the specified resource is busy, [findMeetingTimes](../api/user-findmeetingtimes.md) looks for another resource that is free. If set to false and the specified resource is busy, **findMeetingTimes** returns the resource best ranked in the user's cache without checking if it's free. Default is true.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "locationConstraintItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/locationconstraintitem.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
