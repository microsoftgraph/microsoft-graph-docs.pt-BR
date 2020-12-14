---
title: tipo de recurso printerLocation
description: Representa o local físico e hierárquico de uma impressora.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: bfb082571ab1c5ddf2b46a06c6e66b9e31e47309
ms.sourcegitcommit: 7902607a1e5a030d46e907d08e16644a47a47006
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/12/2020
ms.locfileid: "49664055"
---
# <a name="printerlocation-resource-type"></a><span data-ttu-id="89a30-103">tipo de recurso printerLocation</span><span class="sxs-lookup"><span data-stu-id="89a30-103">printerLocation resource type</span></span>

<span data-ttu-id="89a30-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="89a30-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="89a30-105">Representa o local físico e hierárquico de uma impressora.</span><span class="sxs-lookup"><span data-stu-id="89a30-105">Represents the physical and hierarchical location of a printer.</span></span>

## <a name="properties"></a><span data-ttu-id="89a30-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="89a30-106">Properties</span></span>
| <span data-ttu-id="89a30-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="89a30-107">Property</span></span>     | <span data-ttu-id="89a30-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="89a30-108">Type</span></span>        | <span data-ttu-id="89a30-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="89a30-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="89a30-110">latitude</span><span class="sxs-lookup"><span data-stu-id="89a30-110">latitude</span></span>|<span data-ttu-id="89a30-111">Double</span><span class="sxs-lookup"><span data-stu-id="89a30-111">Double</span></span>|<span data-ttu-id="89a30-112">O Latitude em que a impressora está localizada.</span><span class="sxs-lookup"><span data-stu-id="89a30-112">The latitude that the printer is located at.</span></span>|
|<span data-ttu-id="89a30-113">longitude</span><span class="sxs-lookup"><span data-stu-id="89a30-113">longitude</span></span>|<span data-ttu-id="89a30-114">Double</span><span class="sxs-lookup"><span data-stu-id="89a30-114">Double</span></span>|<span data-ttu-id="89a30-115">A longitude em que a impressora está localizada.</span><span class="sxs-lookup"><span data-stu-id="89a30-115">The longitude that the printer is located at.</span></span>|
|<span data-ttu-id="89a30-116">altitudeInMeters</span><span class="sxs-lookup"><span data-stu-id="89a30-116">altitudeInMeters</span></span>|<span data-ttu-id="89a30-117">Int32</span><span class="sxs-lookup"><span data-stu-id="89a30-117">Int32</span></span>|<span data-ttu-id="89a30-118">A altitude, em metros, em que a impressora está localizada em.</span><span class="sxs-lookup"><span data-stu-id="89a30-118">The altitude, in meters, that the printer is located at.</span></span>|
|<span data-ttu-id="89a30-119">streetAddress</span><span class="sxs-lookup"><span data-stu-id="89a30-119">streetAddress</span></span>|<span data-ttu-id="89a30-120">String</span><span class="sxs-lookup"><span data-stu-id="89a30-120">String</span></span>|<span data-ttu-id="89a30-121">O endereço de rua onde a impressora está localizada.</span><span class="sxs-lookup"><span data-stu-id="89a30-121">The street address where the printer is located.</span></span>|
|<span data-ttu-id="89a30-122">subunidade</span><span class="sxs-lookup"><span data-stu-id="89a30-122">subUnit</span></span>|<span data-ttu-id="89a30-123">String collection</span><span class="sxs-lookup"><span data-stu-id="89a30-123">String collection</span></span>|<span data-ttu-id="89a30-124">A hierarquia de subunidade onde a impressora está localizada.</span><span class="sxs-lookup"><span data-stu-id="89a30-124">The subunit hierarchy where the printer is located.</span></span> <span data-ttu-id="89a30-125">Os elementos devem estar em ordem hierárquica.</span><span class="sxs-lookup"><span data-stu-id="89a30-125">The elements should be in hierarchical order.</span></span> <span data-ttu-id="89a30-126">Por exemplo, se um campus for dividido em seções diferentes, a hierarquia poderá ter a seguinte aparência: `["East Wing", "Block A"]`</span><span class="sxs-lookup"><span data-stu-id="89a30-126">For example, if a campus is divided into different sections, the hierarchy might look like this: `["East Wing", "Block A"]`</span></span>|
|<span data-ttu-id="89a30-127">city</span><span class="sxs-lookup"><span data-stu-id="89a30-127">city</span></span>|<span data-ttu-id="89a30-128">String</span><span class="sxs-lookup"><span data-stu-id="89a30-128">String</span></span>|<span data-ttu-id="89a30-129">A cidade na qual a impressora está localizada.</span><span class="sxs-lookup"><span data-stu-id="89a30-129">The city that the printer is located in.</span></span>|
|<span data-ttu-id="89a30-130">postalCode</span><span class="sxs-lookup"><span data-stu-id="89a30-130">postalCode</span></span>|<span data-ttu-id="89a30-131">String</span><span class="sxs-lookup"><span data-stu-id="89a30-131">String</span></span>|<span data-ttu-id="89a30-132">O CEP em que a impressora está localizada.</span><span class="sxs-lookup"><span data-stu-id="89a30-132">The postal code that the printer is located in.</span></span>|
|<span data-ttu-id="89a30-133">countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="89a30-133">countryOrRegion</span></span>|<span data-ttu-id="89a30-134">String</span><span class="sxs-lookup"><span data-stu-id="89a30-134">String</span></span>|<span data-ttu-id="89a30-135">O país ou a região em que a impressora está localizada.</span><span class="sxs-lookup"><span data-stu-id="89a30-135">The country or region that the printer is located in.</span></span>|
|<span data-ttu-id="89a30-136">site</span><span class="sxs-lookup"><span data-stu-id="89a30-136">site</span></span>|<span data-ttu-id="89a30-137">String</span><span class="sxs-lookup"><span data-stu-id="89a30-137">String</span></span>|<span data-ttu-id="89a30-138">O site no qual a impressora está localizada.</span><span class="sxs-lookup"><span data-stu-id="89a30-138">The site that the printer is located in.</span></span>|
|<span data-ttu-id="89a30-139">Build</span><span class="sxs-lookup"><span data-stu-id="89a30-139">building</span></span>|<span data-ttu-id="89a30-140">String</span><span class="sxs-lookup"><span data-stu-id="89a30-140">String</span></span>|<span data-ttu-id="89a30-141">O edifício em que a impressora está localizada.</span><span class="sxs-lookup"><span data-stu-id="89a30-141">The building that the printer is located in.</span></span>|
|<span data-ttu-id="89a30-142">base</span><span class="sxs-lookup"><span data-stu-id="89a30-142">floor</span></span>|<span data-ttu-id="89a30-143">String</span><span class="sxs-lookup"><span data-stu-id="89a30-143">String</span></span>|<span data-ttu-id="89a30-144">O piso em que a impressora está localizada.</span><span class="sxs-lookup"><span data-stu-id="89a30-144">The floor that the printer is located on.</span></span> <span data-ttu-id="89a30-145">Há suporte apenas para valores numéricos no momento.</span><span class="sxs-lookup"><span data-stu-id="89a30-145">Only numerical values are supported right now.</span></span>|
|<span data-ttu-id="89a30-146">floorDescription</span><span class="sxs-lookup"><span data-stu-id="89a30-146">floorDescription</span></span>|<span data-ttu-id="89a30-147">String</span><span class="sxs-lookup"><span data-stu-id="89a30-147">String</span></span>|<span data-ttu-id="89a30-148">A descrição do piso em que a impressora está localizada.</span><span class="sxs-lookup"><span data-stu-id="89a30-148">The description of the floor that the printer is located on.</span></span>|
|<span data-ttu-id="89a30-149">roomname</span><span class="sxs-lookup"><span data-stu-id="89a30-149">roomName</span></span>|<span data-ttu-id="89a30-150">String</span><span class="sxs-lookup"><span data-stu-id="89a30-150">String</span></span>|<span data-ttu-id="89a30-151">A sala na qual a impressora está localizada.</span><span class="sxs-lookup"><span data-stu-id="89a30-151">The room that the printer is located in.</span></span> <span data-ttu-id="89a30-152">Há suporte apenas para valores numéricos no momento.</span><span class="sxs-lookup"><span data-stu-id="89a30-152">Only numerical values are supported right now.</span></span>|
|<span data-ttu-id="89a30-153">roomDescription</span><span class="sxs-lookup"><span data-stu-id="89a30-153">roomDescription</span></span>|<span data-ttu-id="89a30-154">String</span><span class="sxs-lookup"><span data-stu-id="89a30-154">String</span></span>|<span data-ttu-id="89a30-155">A descrição da sala em que a impressora está localizada.</span><span class="sxs-lookup"><span data-stu-id="89a30-155">The description of the room that the printer is located in.</span></span>|
|<span data-ttu-id="89a30-156">organization</span><span class="sxs-lookup"><span data-stu-id="89a30-156">organization</span></span>|<span data-ttu-id="89a30-157">String collection</span><span class="sxs-lookup"><span data-stu-id="89a30-157">String collection</span></span>|<span data-ttu-id="89a30-158">A hierarquia organizacional à qual a impressora pertence.</span><span class="sxs-lookup"><span data-stu-id="89a30-158">The organizational hierarchy that the printer belongs to.</span></span> <span data-ttu-id="89a30-159">Os elementos devem estar em ordem hierárquica.</span><span class="sxs-lookup"><span data-stu-id="89a30-159">The elements should be in hierarchical order.</span></span>|
|<span data-ttu-id="89a30-160">subdivisão</span><span class="sxs-lookup"><span data-stu-id="89a30-160">subdivision</span></span>|<span data-ttu-id="89a30-161">String collection</span><span class="sxs-lookup"><span data-stu-id="89a30-161">String collection</span></span>|<span data-ttu-id="89a30-162">A subdivisão em que a impressora está localizada.</span><span class="sxs-lookup"><span data-stu-id="89a30-162">The subdivision that the printer is located in.</span></span> <span data-ttu-id="89a30-163">Os elementos devem estar em ordem hierárquica.</span><span class="sxs-lookup"><span data-stu-id="89a30-163">The elements should be in hierarchical order.</span></span>|
|<span data-ttu-id="89a30-164">stateOrProvince</span><span class="sxs-lookup"><span data-stu-id="89a30-164">stateOrProvince</span></span>|<span data-ttu-id="89a30-165">String</span><span class="sxs-lookup"><span data-stu-id="89a30-165">String</span></span>|<span data-ttu-id="89a30-166">O estado ou província em que a impressora está localizada.</span><span class="sxs-lookup"><span data-stu-id="89a30-166">The state or province that the printer is located in.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="89a30-167">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="89a30-167">JSON representation</span></span>

<span data-ttu-id="89a30-168">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="89a30-168">The following is a JSON representation of the resource.</span></span>

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
    "floor": "123456",
    "floorDescription": "String",
    "roomName": "123456",
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

