---
title: Tipo de recurso locationConstraintItem
description: As condições indicadas por um cliente para o local de uma reunião.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: ecc29f65cf8296250c3daceddc8b7b5ca1a88381
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345222"
---
# <a name="locationconstraintitem-resource-type"></a><span data-ttu-id="f8227-103">Tipo de recurso locationConstraintItem</span><span class="sxs-lookup"><span data-stu-id="f8227-103">locationConstraintItem resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f8227-104">As condições indicadas por um cliente para o local de uma reunião.</span><span class="sxs-lookup"><span data-stu-id="f8227-104">The conditions stated by a client for the location of a meeting.</span></span>

<span data-ttu-id="f8227-105">Derivado de [location](location.md).</span><span class="sxs-lookup"><span data-stu-id="f8227-105">Derived from [location](location.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="f8227-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f8227-106">JSON representation</span></span>

<span data-ttu-id="f8227-107">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="f8227-107">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="f8227-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f8227-108">Properties</span></span>
| <span data-ttu-id="f8227-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f8227-109">Property</span></span>     | <span data-ttu-id="f8227-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="f8227-110">Type</span></span>   |<span data-ttu-id="f8227-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="f8227-111">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="f8227-112">address</span><span class="sxs-lookup"><span data-stu-id="f8227-112">address</span></span> | [<span data-ttu-id="f8227-113">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="f8227-113">physicalAddress</span></span>](physicaladdress.md) |<span data-ttu-id="f8227-114">O endereço físico do local.</span><span class="sxs-lookup"><span data-stu-id="f8227-114">The street address of the location.</span></span> |
| <span data-ttu-id="f8227-115">coordenadas</span><span class="sxs-lookup"><span data-stu-id="f8227-115">coordinates</span></span> | [<span data-ttu-id="f8227-116">outlookGeoCoordinates</span><span class="sxs-lookup"><span data-stu-id="f8227-116">outlookGeoCoordinates</span></span>](outlookgeocoordinates.md) | <span data-ttu-id="f8227-117">As coordenadas geográficas e a elevação do local.</span><span class="sxs-lookup"><span data-stu-id="f8227-117">The geographic coordinates and elevation of the location.</span></span> |
| <span data-ttu-id="f8227-118">displayName</span><span class="sxs-lookup"><span data-stu-id="f8227-118">displayName</span></span>  | <span data-ttu-id="f8227-119">String</span><span class="sxs-lookup"><span data-stu-id="f8227-119">String</span></span> | <span data-ttu-id="f8227-120">O nome associado ao local.</span><span class="sxs-lookup"><span data-stu-id="f8227-120">The name associated with the location.</span></span>                       |
| <span data-ttu-id="f8227-121">locationEmailAddress</span><span class="sxs-lookup"><span data-stu-id="f8227-121">locationEmailAddress</span></span> | <span data-ttu-id="f8227-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f8227-122">String</span></span> | <span data-ttu-id="f8227-123">O endereço de email opcional do local.</span><span class="sxs-lookup"><span data-stu-id="f8227-123">Optional email address of the location.</span></span> |
| <span data-ttu-id="f8227-124">locationType</span><span class="sxs-lookup"><span data-stu-id="f8227-124">locationType</span></span> | <span data-ttu-id="f8227-125">locationType</span><span class="sxs-lookup"><span data-stu-id="f8227-125">locationType</span></span> | <span data-ttu-id="f8227-126">O tipo de local.</span><span class="sxs-lookup"><span data-stu-id="f8227-126">The type of location.</span></span> <span data-ttu-id="f8227-127">Os valores possíveis são: `default`, `conferenceRoom`, `homeAddress`, `businessAddress`,`geoCoordinates`, `streetAddress`, `hotel`, `restaurant`, `localBusiness`, `postalAddress`.</span><span class="sxs-lookup"><span data-stu-id="f8227-127">Possible values are: `default`, `conferenceRoom`, `homeAddress`, `businessAddress`,`geoCoordinates`, `streetAddress`, `hotel`, `restaurant`, `localBusiness`, `postalAddress`.</span></span> <span data-ttu-id="f8227-128">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f8227-128">Read-only.</span></span>|
| <span data-ttu-id="f8227-129">locationUri</span><span class="sxs-lookup"><span data-stu-id="f8227-129">locationUri</span></span> | <span data-ttu-id="f8227-130">String</span><span class="sxs-lookup"><span data-stu-id="f8227-130">String</span></span> | <span data-ttu-id="f8227-131">URI opcional que representa o local.</span><span class="sxs-lookup"><span data-stu-id="f8227-131">Optional URI representing the location.</span></span> |
| <span data-ttu-id="f8227-132">resolveAvailability</span><span class="sxs-lookup"><span data-stu-id="f8227-132">resolveAvailability</span></span> | <span data-ttu-id="f8227-133">Booliano</span><span class="sxs-lookup"><span data-stu-id="f8227-133">Boolean</span></span> | <span data-ttu-id="f8227-p102">Se definido como true e o recurso especificado está ocupado, [findMeetingTimes](../api/user-findmeetingtimes.md) procura outro recurso livre. Se definido como false e o recurso especificado está ocupado, **findMeetingTimes** retorna o recurso melhor classificado no cache do usuário sem verificar se ele está livre. O padrão é true.</span><span class="sxs-lookup"><span data-stu-id="f8227-p102">If set to true and the specified resource is busy, [findMeetingTimes](../api/user-findmeetingtimes.md) looks for another resource that is free. If set to false and the specified resource is busy, **findMeetingTimes** returns the resource best ranked in the user's cache without checking if it's free. Default is true.</span></span> |
| <span data-ttu-id="f8227-137">uniqueId</span><span class="sxs-lookup"><span data-stu-id="f8227-137">uniqueId</span></span> | <span data-ttu-id="f8227-138">String</span><span class="sxs-lookup"><span data-stu-id="f8227-138">String</span></span> | <span data-ttu-id="f8227-139">Apenas para uso interno.</span><span class="sxs-lookup"><span data-stu-id="f8227-139">For internal use only.</span></span>|
| <span data-ttu-id="f8227-140">uniqueIdType</span><span class="sxs-lookup"><span data-stu-id="f8227-140">uniqueIdType</span></span> | <span data-ttu-id="f8227-141">String</span><span class="sxs-lookup"><span data-stu-id="f8227-141">String</span></span> | <span data-ttu-id="f8227-142">Apenas para uso interno.</span><span class="sxs-lookup"><span data-stu-id="f8227-142">For internal use only.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "locationConstraintItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
