---
title: Tipo de recurso locationConstraintItem
description: As condições indicadas por um cliente para o local de uma reunião.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 7063eb0a7aa437b51a2bfecb482012771297f766
ms.sourcegitcommit: a90abf5b89dbbdfefb1b7794d1f12c6e2bfb0cda
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/28/2019
ms.locfileid: "30936252"
---
# <a name="locationconstraintitem-resource-type"></a><span data-ttu-id="f7757-103">Tipo de recurso locationConstraintItem</span><span class="sxs-lookup"><span data-stu-id="f7757-103">locationConstraintItem resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f7757-104">As condições indicadas por um cliente para o local de uma reunião.</span><span class="sxs-lookup"><span data-stu-id="f7757-104">The conditions stated by a client for the location of a meeting.</span></span>

<span data-ttu-id="f7757-105">Derivado de [location](location.md).</span><span class="sxs-lookup"><span data-stu-id="f7757-105">Derived from [location](location.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="f7757-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f7757-106">JSON representation</span></span>

<span data-ttu-id="f7757-107">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="f7757-107">Here is a JSON representation of the resource</span></span>

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
  "locationType": "string",
  "locationUri": "string",
  "uniqueId": "string",
  "uniqueIdType": "string"
}

```
## <a name="properties"></a><span data-ttu-id="f7757-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f7757-108">Properties</span></span>
| <span data-ttu-id="f7757-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f7757-109">Property</span></span>     | <span data-ttu-id="f7757-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="f7757-110">Type</span></span>   |<span data-ttu-id="f7757-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="f7757-111">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="f7757-112">address</span><span class="sxs-lookup"><span data-stu-id="f7757-112">address</span></span> | [<span data-ttu-id="f7757-113">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="f7757-113">physicalAddress</span></span>](physicaladdress.md) |<span data-ttu-id="f7757-114">O endereço físico do local.</span><span class="sxs-lookup"><span data-stu-id="f7757-114">The street address of the location.</span></span> |
| <span data-ttu-id="f7757-115">coordenadas</span><span class="sxs-lookup"><span data-stu-id="f7757-115">coordinates</span></span> | [<span data-ttu-id="f7757-116">outlookGeoCoordinates</span><span class="sxs-lookup"><span data-stu-id="f7757-116">outlookGeoCoordinates</span></span>](outlookgeocoordinates.md) | <span data-ttu-id="f7757-117">As coordenadas geográficas e a elevação do local.</span><span class="sxs-lookup"><span data-stu-id="f7757-117">The geographic coordinates and elevation of the location.</span></span> |
| <span data-ttu-id="f7757-118">displayName</span><span class="sxs-lookup"><span data-stu-id="f7757-118">displayName</span></span>  | <span data-ttu-id="f7757-119">String</span><span class="sxs-lookup"><span data-stu-id="f7757-119">String</span></span> | <span data-ttu-id="f7757-120">O nome associado ao local.</span><span class="sxs-lookup"><span data-stu-id="f7757-120">The name associated with the location.</span></span>                       |
| <span data-ttu-id="f7757-121">locationEmailAddress</span><span class="sxs-lookup"><span data-stu-id="f7757-121">locationEmailAddress</span></span> | <span data-ttu-id="f7757-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f7757-122">String</span></span> | <span data-ttu-id="f7757-123">O endereço de email opcional do local.</span><span class="sxs-lookup"><span data-stu-id="f7757-123">Optional email address of the location.</span></span> |
| <span data-ttu-id="f7757-124">locationType</span><span class="sxs-lookup"><span data-stu-id="f7757-124">locationType</span></span> | <span data-ttu-id="f7757-125">locationType</span><span class="sxs-lookup"><span data-stu-id="f7757-125">locationType</span></span> | <span data-ttu-id="f7757-126">O tipo de local.</span><span class="sxs-lookup"><span data-stu-id="f7757-126">The type of location.</span></span> <span data-ttu-id="f7757-127">Os valores possíveis são: `default`, `conferenceRoom`, `homeAddress`, `businessAddress`,`geoCoordinates`, `streetAddress`, `hotel`, `restaurant`, `localBusiness`, `postalAddress`.</span><span class="sxs-lookup"><span data-stu-id="f7757-127">Possible values are: `default`, `conferenceRoom`, `homeAddress`, `businessAddress`,`geoCoordinates`, `streetAddress`, `hotel`, `restaurant`, `localBusiness`, `postalAddress`.</span></span> <span data-ttu-id="f7757-128">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f7757-128">Read-only.</span></span>|
| <span data-ttu-id="f7757-129">locationUri</span><span class="sxs-lookup"><span data-stu-id="f7757-129">locationUri</span></span> | <span data-ttu-id="f7757-130">String</span><span class="sxs-lookup"><span data-stu-id="f7757-130">String</span></span> | <span data-ttu-id="f7757-131">URI opcional que representa o local.</span><span class="sxs-lookup"><span data-stu-id="f7757-131">Optional URI representing the location.</span></span> |
| <span data-ttu-id="f7757-132">resolveAvailability</span><span class="sxs-lookup"><span data-stu-id="f7757-132">resolveAvailability</span></span> | <span data-ttu-id="f7757-133">Booliano</span><span class="sxs-lookup"><span data-stu-id="f7757-133">Boolean</span></span> | <span data-ttu-id="f7757-p102">Se definido como true e o recurso especificado está ocupado, [findMeetingTimes](../api/user-findmeetingtimes.md) procura outro recurso livre. Se definido como false e o recurso especificado está ocupado, **findMeetingTimes** retorna o recurso melhor classificado no cache do usuário sem verificar se ele está livre. O padrão é true.</span><span class="sxs-lookup"><span data-stu-id="f7757-p102">If set to true and the specified resource is busy, [findMeetingTimes](../api/user-findmeetingtimes.md) looks for another resource that is free. If set to false and the specified resource is busy, **findMeetingTimes** returns the resource best ranked in the user's cache without checking if it's free. Default is true.</span></span> |
| <span data-ttu-id="f7757-137">uniqueId</span><span class="sxs-lookup"><span data-stu-id="f7757-137">uniqueId</span></span> | <span data-ttu-id="f7757-138">String</span><span class="sxs-lookup"><span data-stu-id="f7757-138">String</span></span> | <span data-ttu-id="f7757-139">Apenas para uso interno.</span><span class="sxs-lookup"><span data-stu-id="f7757-139">For internal use only.</span></span>|
| <span data-ttu-id="f7757-140">uniqueIdType</span><span class="sxs-lookup"><span data-stu-id="f7757-140">uniqueIdType</span></span> | <span data-ttu-id="f7757-141">String</span><span class="sxs-lookup"><span data-stu-id="f7757-141">String</span></span> | <span data-ttu-id="f7757-142">Apenas para uso interno.</span><span class="sxs-lookup"><span data-stu-id="f7757-142">For internal use only.</span></span> |

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
