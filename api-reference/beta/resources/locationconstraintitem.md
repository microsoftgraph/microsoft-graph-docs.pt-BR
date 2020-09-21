---
title: Tipo de recurso locationConstraintItem
description: As condições indicadas por um cliente para o local de uma reunião.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 58c05dadf30399ef704980b3bbbf24ac74330f6e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48058092"
---
# <a name="locationconstraintitem-resource-type"></a><span data-ttu-id="235d4-103">Tipo de recurso locationConstraintItem</span><span class="sxs-lookup"><span data-stu-id="235d4-103">locationConstraintItem resource type</span></span>

<span data-ttu-id="235d4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="235d4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="235d4-105">As condições indicadas por um cliente para o local de uma reunião.</span><span class="sxs-lookup"><span data-stu-id="235d4-105">The conditions stated by a client for the location of a meeting.</span></span>

<span data-ttu-id="235d4-106">Derivado de [location](location.md).</span><span class="sxs-lookup"><span data-stu-id="235d4-106">Derived from [location](location.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="235d4-107">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="235d4-107">JSON representation</span></span>

<span data-ttu-id="235d4-108">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="235d4-108">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="235d4-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="235d4-109">Properties</span></span>
| <span data-ttu-id="235d4-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="235d4-110">Property</span></span>     | <span data-ttu-id="235d4-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="235d4-111">Type</span></span>   |<span data-ttu-id="235d4-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="235d4-112">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="235d4-113">address</span><span class="sxs-lookup"><span data-stu-id="235d4-113">address</span></span> | [<span data-ttu-id="235d4-114">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="235d4-114">physicalAddress</span></span>](physicaladdress.md) |<span data-ttu-id="235d4-115">O endereço físico do local.</span><span class="sxs-lookup"><span data-stu-id="235d4-115">The street address of the location.</span></span> |
| <span data-ttu-id="235d4-116">coordenadas</span><span class="sxs-lookup"><span data-stu-id="235d4-116">coordinates</span></span> | [<span data-ttu-id="235d4-117">outlookGeoCoordinates</span><span class="sxs-lookup"><span data-stu-id="235d4-117">outlookGeoCoordinates</span></span>](outlookgeocoordinates.md) | <span data-ttu-id="235d4-118">As coordenadas geográficas e a elevação do local.</span><span class="sxs-lookup"><span data-stu-id="235d4-118">The geographic coordinates and elevation of the location.</span></span> |
| <span data-ttu-id="235d4-119">displayName</span><span class="sxs-lookup"><span data-stu-id="235d4-119">displayName</span></span>  | <span data-ttu-id="235d4-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="235d4-120">String</span></span> | <span data-ttu-id="235d4-121">O nome associado ao local.</span><span class="sxs-lookup"><span data-stu-id="235d4-121">The name associated with the location.</span></span>                       |
| <span data-ttu-id="235d4-122">locationEmailAddress</span><span class="sxs-lookup"><span data-stu-id="235d4-122">locationEmailAddress</span></span> | <span data-ttu-id="235d4-123">String</span><span class="sxs-lookup"><span data-stu-id="235d4-123">String</span></span> | <span data-ttu-id="235d4-124">O endereço de email opcional do local.</span><span class="sxs-lookup"><span data-stu-id="235d4-124">Optional email address of the location.</span></span> |
| <span data-ttu-id="235d4-125">locationType</span><span class="sxs-lookup"><span data-stu-id="235d4-125">locationType</span></span> | <span data-ttu-id="235d4-126">locationType</span><span class="sxs-lookup"><span data-stu-id="235d4-126">locationType</span></span> | <span data-ttu-id="235d4-127">O tipo de local.</span><span class="sxs-lookup"><span data-stu-id="235d4-127">The type of location.</span></span> <span data-ttu-id="235d4-128">Os valores possíveis são: `default`, `conferenceRoom`, `homeAddress`, `businessAddress`,`geoCoordinates`, `streetAddress`, `hotel`, `restaurant`, `localBusiness`, `postalAddress`.</span><span class="sxs-lookup"><span data-stu-id="235d4-128">Possible values are: `default`, `conferenceRoom`, `homeAddress`, `businessAddress`,`geoCoordinates`, `streetAddress`, `hotel`, `restaurant`, `localBusiness`, `postalAddress`.</span></span> <span data-ttu-id="235d4-129">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="235d4-129">Read-only.</span></span>|
| <span data-ttu-id="235d4-130">locationUri</span><span class="sxs-lookup"><span data-stu-id="235d4-130">locationUri</span></span> | <span data-ttu-id="235d4-131">String</span><span class="sxs-lookup"><span data-stu-id="235d4-131">String</span></span> | <span data-ttu-id="235d4-132">URI opcional que representa o local.</span><span class="sxs-lookup"><span data-stu-id="235d4-132">Optional URI representing the location.</span></span> |
| <span data-ttu-id="235d4-133">resolveAvailability</span><span class="sxs-lookup"><span data-stu-id="235d4-133">resolveAvailability</span></span> | <span data-ttu-id="235d4-134">Booliano</span><span class="sxs-lookup"><span data-stu-id="235d4-134">Boolean</span></span> | <span data-ttu-id="235d4-p102">Se definido como true e o recurso especificado está ocupado, [findMeetingTimes](../api/user-findmeetingtimes.md) procura outro recurso livre. Se definido como false e o recurso especificado está ocupado, **findMeetingTimes** retorna o recurso melhor classificado no cache do usuário sem verificar se ele está livre. O padrão é true.</span><span class="sxs-lookup"><span data-stu-id="235d4-p102">If set to true and the specified resource is busy, [findMeetingTimes](../api/user-findmeetingtimes.md) looks for another resource that is free. If set to false and the specified resource is busy, **findMeetingTimes** returns the resource best ranked in the user's cache without checking if it's free. Default is true.</span></span> |
| <span data-ttu-id="235d4-138">uniqueId</span><span class="sxs-lookup"><span data-stu-id="235d4-138">uniqueId</span></span> | <span data-ttu-id="235d4-139">String</span><span class="sxs-lookup"><span data-stu-id="235d4-139">String</span></span> | <span data-ttu-id="235d4-140">Apenas para uso interno.</span><span class="sxs-lookup"><span data-stu-id="235d4-140">For internal use only.</span></span>|
| <span data-ttu-id="235d4-141">uniqueIdType</span><span class="sxs-lookup"><span data-stu-id="235d4-141">uniqueIdType</span></span> | <span data-ttu-id="235d4-142">String</span><span class="sxs-lookup"><span data-stu-id="235d4-142">String</span></span> | <span data-ttu-id="235d4-143">Apenas para uso interno.</span><span class="sxs-lookup"><span data-stu-id="235d4-143">For internal use only.</span></span> |

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


