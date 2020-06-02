---
title: tipo de recurso printerLocation
description: Representa o local físico e hierárquico de uma impressora.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: b8fd40de56d97f70a6208cf68a56c74d711eb78e
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44251090"
---
# <a name="printerlocation-resource-type"></a><span data-ttu-id="34d8b-103">tipo de recurso printerLocation</span><span class="sxs-lookup"><span data-stu-id="34d8b-103">printerLocation resource type</span></span>

<span data-ttu-id="34d8b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="34d8b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="34d8b-105">Representa o local físico e hierárquico de uma impressora.</span><span class="sxs-lookup"><span data-stu-id="34d8b-105">Represents the physical and hierarchical location of a printer.</span></span>

## <a name="properties"></a><span data-ttu-id="34d8b-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="34d8b-106">Properties</span></span>
| <span data-ttu-id="34d8b-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="34d8b-107">Property</span></span>     | <span data-ttu-id="34d8b-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="34d8b-108">Type</span></span>        | <span data-ttu-id="34d8b-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="34d8b-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="34d8b-110">latitude</span><span class="sxs-lookup"><span data-stu-id="34d8b-110">latitude</span></span>|<span data-ttu-id="34d8b-111">Duplo</span><span class="sxs-lookup"><span data-stu-id="34d8b-111">Double</span></span>|<span data-ttu-id="34d8b-112">O Latitude em que a impressora está localizada.</span><span class="sxs-lookup"><span data-stu-id="34d8b-112">The latitude that the printer is located at.</span></span>|
|<span data-ttu-id="34d8b-113">longitude</span><span class="sxs-lookup"><span data-stu-id="34d8b-113">longitude</span></span>|<span data-ttu-id="34d8b-114">Double</span><span class="sxs-lookup"><span data-stu-id="34d8b-114">Double</span></span>|<span data-ttu-id="34d8b-115">A longitude em que a impressora está localizada.</span><span class="sxs-lookup"><span data-stu-id="34d8b-115">The longitude that the printer is located at.</span></span>|
|<span data-ttu-id="34d8b-116">altitudeInMeters</span><span class="sxs-lookup"><span data-stu-id="34d8b-116">altitudeInMeters</span></span>|<span data-ttu-id="34d8b-117">Int32</span><span class="sxs-lookup"><span data-stu-id="34d8b-117">Int32</span></span>|<span data-ttu-id="34d8b-118">A altitude, em metros, em que a impressora está localizada em.</span><span class="sxs-lookup"><span data-stu-id="34d8b-118">The altitude, in meters, that the printer is located at.</span></span>|
|<span data-ttu-id="34d8b-119">streetAddress</span><span class="sxs-lookup"><span data-stu-id="34d8b-119">streetAddress</span></span>|<span data-ttu-id="34d8b-120">String</span><span class="sxs-lookup"><span data-stu-id="34d8b-120">String</span></span>|<span data-ttu-id="34d8b-121">O endereço de rua onde a impressora está localizada.</span><span class="sxs-lookup"><span data-stu-id="34d8b-121">The street address where the printer is located.</span></span>|
|<span data-ttu-id="34d8b-122">subunidade</span><span class="sxs-lookup"><span data-stu-id="34d8b-122">subUnit</span></span>|<span data-ttu-id="34d8b-123">Conjunto de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="34d8b-123">String collection</span></span>|<span data-ttu-id="34d8b-124">A hierarquia de subunidade onde a impressora está localizada.</span><span class="sxs-lookup"><span data-stu-id="34d8b-124">The subunit hierarchy where the printer is located.</span></span> <span data-ttu-id="34d8b-125">Os elementos devem estar em ordem hierárquica.</span><span class="sxs-lookup"><span data-stu-id="34d8b-125">The elements should be in hierarchical order.</span></span> <span data-ttu-id="34d8b-126">Por exemplo, se um campus for dividido em seções diferentes, a hierarquia poderá ter a seguinte aparência:`["East Wing", "Block A"]`</span><span class="sxs-lookup"><span data-stu-id="34d8b-126">For example, if a campus is divided into different sections, the hierarchy might look like this: `["East Wing", "Block A"]`</span></span>|
|<span data-ttu-id="34d8b-127">city</span><span class="sxs-lookup"><span data-stu-id="34d8b-127">city</span></span>|<span data-ttu-id="34d8b-128">String</span><span class="sxs-lookup"><span data-stu-id="34d8b-128">String</span></span>|<span data-ttu-id="34d8b-129">A cidade na qual a impressora está localizada.</span><span class="sxs-lookup"><span data-stu-id="34d8b-129">The city that the printer is located in.</span></span>|
|<span data-ttu-id="34d8b-130">postalCode</span><span class="sxs-lookup"><span data-stu-id="34d8b-130">postalCode</span></span>|<span data-ttu-id="34d8b-131">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="34d8b-131">String</span></span>|<span data-ttu-id="34d8b-132">O CEP em que a impressora está localizada.</span><span class="sxs-lookup"><span data-stu-id="34d8b-132">The postal code that the printer is located in.</span></span>|
|<span data-ttu-id="34d8b-133">countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="34d8b-133">countryOrRegion</span></span>|<span data-ttu-id="34d8b-134">String</span><span class="sxs-lookup"><span data-stu-id="34d8b-134">String</span></span>|<span data-ttu-id="34d8b-135">O país ou a região em que a impressora está localizada.</span><span class="sxs-lookup"><span data-stu-id="34d8b-135">The country or region that the printer is located in.</span></span>|
|<span data-ttu-id="34d8b-136">site</span><span class="sxs-lookup"><span data-stu-id="34d8b-136">site</span></span>|<span data-ttu-id="34d8b-137">String</span><span class="sxs-lookup"><span data-stu-id="34d8b-137">String</span></span>|<span data-ttu-id="34d8b-138">O site no qual a impressora está localizada.</span><span class="sxs-lookup"><span data-stu-id="34d8b-138">The site that the printer is located in.</span></span>|
|<span data-ttu-id="34d8b-139">Build</span><span class="sxs-lookup"><span data-stu-id="34d8b-139">building</span></span>|<span data-ttu-id="34d8b-140">String</span><span class="sxs-lookup"><span data-stu-id="34d8b-140">String</span></span>|<span data-ttu-id="34d8b-141">O edifício em que a impressora está localizada.</span><span class="sxs-lookup"><span data-stu-id="34d8b-141">The building that the printer is located in.</span></span>|
|<span data-ttu-id="34d8b-142">floorNumber</span><span class="sxs-lookup"><span data-stu-id="34d8b-142">floorNumber</span></span>|<span data-ttu-id="34d8b-143">Int32</span><span class="sxs-lookup"><span data-stu-id="34d8b-143">Int32</span></span>|<span data-ttu-id="34d8b-144">O número do andar em que a impressora está localizada.</span><span class="sxs-lookup"><span data-stu-id="34d8b-144">The floor number that the printer is located on.</span></span>|
|<span data-ttu-id="34d8b-145">floorDescription</span><span class="sxs-lookup"><span data-stu-id="34d8b-145">floorDescription</span></span>|<span data-ttu-id="34d8b-146">String</span><span class="sxs-lookup"><span data-stu-id="34d8b-146">String</span></span>|<span data-ttu-id="34d8b-147">A descrição do piso em que a impressora está localizada.</span><span class="sxs-lookup"><span data-stu-id="34d8b-147">The description of the floor that the printer is located on.</span></span>|
|<span data-ttu-id="34d8b-148">Númerodasala</span><span class="sxs-lookup"><span data-stu-id="34d8b-148">roomNumber</span></span>|<span data-ttu-id="34d8b-149">Int32</span><span class="sxs-lookup"><span data-stu-id="34d8b-149">Int32</span></span>|<span data-ttu-id="34d8b-150">O número da sala em que a impressora está localizada.</span><span class="sxs-lookup"><span data-stu-id="34d8b-150">The room number that the printer is located in.</span></span>|
|<span data-ttu-id="34d8b-151">roomDescription</span><span class="sxs-lookup"><span data-stu-id="34d8b-151">roomDescription</span></span>|<span data-ttu-id="34d8b-152">String</span><span class="sxs-lookup"><span data-stu-id="34d8b-152">String</span></span>|<span data-ttu-id="34d8b-153">A descrição da sala em que a impressora está localizada.</span><span class="sxs-lookup"><span data-stu-id="34d8b-153">The description of the room that the printer is located in.</span></span>|
|<span data-ttu-id="34d8b-154">organization</span><span class="sxs-lookup"><span data-stu-id="34d8b-154">organization</span></span>|<span data-ttu-id="34d8b-155">Conjunto de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="34d8b-155">String collection</span></span>|<span data-ttu-id="34d8b-156">A hierarquia organizacional à qual a impressora pertence.</span><span class="sxs-lookup"><span data-stu-id="34d8b-156">The organizational hierarchy that the printer belongs to.</span></span> <span data-ttu-id="34d8b-157">Os elementos devem estar em ordem hierárquica.</span><span class="sxs-lookup"><span data-stu-id="34d8b-157">The elements should be in hierarchical order.</span></span>|
|<span data-ttu-id="34d8b-158">subdivisão</span><span class="sxs-lookup"><span data-stu-id="34d8b-158">subdivision</span></span>|<span data-ttu-id="34d8b-159">Conjunto de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="34d8b-159">String collection</span></span>|<span data-ttu-id="34d8b-160">A subdivisão em que a impressora está localizada.</span><span class="sxs-lookup"><span data-stu-id="34d8b-160">The subdivision that the printer is located in.</span></span> <span data-ttu-id="34d8b-161">Os elementos devem estar em ordem hierárquica.</span><span class="sxs-lookup"><span data-stu-id="34d8b-161">The elements should be in hierarchical order.</span></span>|
|<span data-ttu-id="34d8b-162">stateOrProvince</span><span class="sxs-lookup"><span data-stu-id="34d8b-162">stateOrProvince</span></span>|<span data-ttu-id="34d8b-163">String</span><span class="sxs-lookup"><span data-stu-id="34d8b-163">String</span></span>|<span data-ttu-id="34d8b-164">O estado ou província em que a impressora está localizada.</span><span class="sxs-lookup"><span data-stu-id="34d8b-164">The state or province that the printer is located in.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="34d8b-165">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="34d8b-165">JSON representation</span></span>

<span data-ttu-id="34d8b-166">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="34d8b-166">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printerLocation"
}-->

```json
{
    "latitude": 80.1,
    "longitude": -170.1,
    "altitudeInMeters": 123456,
    "streetAddress": "String",
    "subUnit": ["String"],
    "city": "String",
    "postalCode": "String",
    "countryOrRegion": "String",
    "site": "String",
    "building": "String",
    "floorNumber": 123456,
    "floorDescription": "String",
    "roomNumber": 123456,
    "roomDescription": "String",
    "organization": ["String"],
    "subdivision": ["String"],
    "stateOrProvince": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printerLocation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->