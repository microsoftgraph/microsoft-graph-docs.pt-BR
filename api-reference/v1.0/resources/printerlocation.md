---
title: Tipo de recurso printerLocation
description: Representa o local físico e hierárquico de uma impressora.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: f357ab3b33182ac6ffb2f8ae705a359a0e955eed
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/06/2021
ms.locfileid: "50516831"
---
# <a name="printerlocation-resource-type"></a><span data-ttu-id="fb4f8-103">Tipo de recurso printerLocation</span><span class="sxs-lookup"><span data-stu-id="fb4f8-103">printerLocation resource type</span></span>

<span data-ttu-id="fb4f8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fb4f8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="fb4f8-105">Representa o local físico e hierárquico de uma impressora.</span><span class="sxs-lookup"><span data-stu-id="fb4f8-105">Represents the physical and hierarchical location of a printer.</span></span>

## <a name="properties"></a><span data-ttu-id="fb4f8-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fb4f8-106">Properties</span></span>
|<span data-ttu-id="fb4f8-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fb4f8-107">Property</span></span>|<span data-ttu-id="fb4f8-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="fb4f8-108">Type</span></span>|<span data-ttu-id="fb4f8-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="fb4f8-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fb4f8-110">latitude</span><span class="sxs-lookup"><span data-stu-id="fb4f8-110">latitude</span></span>|<span data-ttu-id="fb4f8-111">Double</span><span class="sxs-lookup"><span data-stu-id="fb4f8-111">Double</span></span>|<span data-ttu-id="fb4f8-112">A latitude em que a impressora está localizada.</span><span class="sxs-lookup"><span data-stu-id="fb4f8-112">The latitude that the printer is located at.</span></span>|
|<span data-ttu-id="fb4f8-113">longitude</span><span class="sxs-lookup"><span data-stu-id="fb4f8-113">longitude</span></span>|<span data-ttu-id="fb4f8-114">Double</span><span class="sxs-lookup"><span data-stu-id="fb4f8-114">Double</span></span>|<span data-ttu-id="fb4f8-115">A longitude em que a impressora está localizada.</span><span class="sxs-lookup"><span data-stu-id="fb4f8-115">The longitude that the printer is located at.</span></span>|
|<span data-ttu-id="fb4f8-116">altitudeInMeters</span><span class="sxs-lookup"><span data-stu-id="fb4f8-116">altitudeInMeters</span></span>|<span data-ttu-id="fb4f8-117">Int32</span><span class="sxs-lookup"><span data-stu-id="fb4f8-117">Int32</span></span>|<span data-ttu-id="fb4f8-118">A altitude, em metros, em que a impressora está localizada.</span><span class="sxs-lookup"><span data-stu-id="fb4f8-118">The altitude, in meters, that the printer is located at.</span></span>|
|<span data-ttu-id="fb4f8-119">streetAddress</span><span class="sxs-lookup"><span data-stu-id="fb4f8-119">streetAddress</span></span>|<span data-ttu-id="fb4f8-120">String</span><span class="sxs-lookup"><span data-stu-id="fb4f8-120">String</span></span>|<span data-ttu-id="fb4f8-121">O endereço de rua onde a impressora está localizada.</span><span class="sxs-lookup"><span data-stu-id="fb4f8-121">The street address where the printer is located.</span></span>|
|<span data-ttu-id="fb4f8-122">subUnit</span><span class="sxs-lookup"><span data-stu-id="fb4f8-122">subUnit</span></span>|<span data-ttu-id="fb4f8-123">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="fb4f8-123">String collection</span></span>|<span data-ttu-id="fb4f8-124">A hierarquia de subunidades onde a impressora está localizada.</span><span class="sxs-lookup"><span data-stu-id="fb4f8-124">The subunit hierarchy where the printer is located.</span></span> <span data-ttu-id="fb4f8-125">Os elementos devem estar em ordem hierárquica.</span><span class="sxs-lookup"><span data-stu-id="fb4f8-125">The elements should be in hierarchical order.</span></span> <span data-ttu-id="fb4f8-126">Por exemplo, se um campus for dividido em seções diferentes, a hierarquia poderá ter esta aparência: `["East Wing", "Block A"]`</span><span class="sxs-lookup"><span data-stu-id="fb4f8-126">For example, if a campus is divided into different sections, the hierarchy might look like this: `["East Wing", "Block A"]`</span></span>|
|<span data-ttu-id="fb4f8-127">city</span><span class="sxs-lookup"><span data-stu-id="fb4f8-127">city</span></span>|<span data-ttu-id="fb4f8-128">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fb4f8-128">String</span></span>|<span data-ttu-id="fb4f8-129">A cidade em que a impressora está localizada.</span><span class="sxs-lookup"><span data-stu-id="fb4f8-129">The city that the printer is located in.</span></span>|
|<span data-ttu-id="fb4f8-130">postalCode</span><span class="sxs-lookup"><span data-stu-id="fb4f8-130">postalCode</span></span>|<span data-ttu-id="fb4f8-131">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fb4f8-131">String</span></span>|<span data-ttu-id="fb4f8-132">O código postal em que a impressora está localizada.</span><span class="sxs-lookup"><span data-stu-id="fb4f8-132">The postal code that the printer is located in.</span></span>|
|<span data-ttu-id="fb4f8-133">countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="fb4f8-133">countryOrRegion</span></span>|<span data-ttu-id="fb4f8-134">String</span><span class="sxs-lookup"><span data-stu-id="fb4f8-134">String</span></span>|<span data-ttu-id="fb4f8-135">O país ou a região em que a impressora está localizada.</span><span class="sxs-lookup"><span data-stu-id="fb4f8-135">The country or region that the printer is located in.</span></span>|
|<span data-ttu-id="fb4f8-136">site</span><span class="sxs-lookup"><span data-stu-id="fb4f8-136">site</span></span>|<span data-ttu-id="fb4f8-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fb4f8-137">String</span></span>|<span data-ttu-id="fb4f8-138">O site em que a impressora está localizada.</span><span class="sxs-lookup"><span data-stu-id="fb4f8-138">The site that the printer is located in.</span></span>|
|<span data-ttu-id="fb4f8-139">building</span><span class="sxs-lookup"><span data-stu-id="fb4f8-139">building</span></span>|<span data-ttu-id="fb4f8-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fb4f8-140">String</span></span>|<span data-ttu-id="fb4f8-141">O edifício em que a impressora está localizada.</span><span class="sxs-lookup"><span data-stu-id="fb4f8-141">The building that the printer is located in.</span></span>|
|<span data-ttu-id="fb4f8-142">base</span><span class="sxs-lookup"><span data-stu-id="fb4f8-142">floor</span></span>|<span data-ttu-id="fb4f8-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fb4f8-143">String</span></span>|<span data-ttu-id="fb4f8-144">O piso no que a impressora está localizada.</span><span class="sxs-lookup"><span data-stu-id="fb4f8-144">The floor that the printer is located on.</span></span> <span data-ttu-id="fb4f8-145">Somente valores numéricos são suportados no momento.</span><span class="sxs-lookup"><span data-stu-id="fb4f8-145">Only numerical values are supported right now.</span></span>|
|<span data-ttu-id="fb4f8-146">floorDescription</span><span class="sxs-lookup"><span data-stu-id="fb4f8-146">floorDescription</span></span>|<span data-ttu-id="fb4f8-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fb4f8-147">String</span></span>|<span data-ttu-id="fb4f8-148">A descrição do piso em que a impressora está localizada.</span><span class="sxs-lookup"><span data-stu-id="fb4f8-148">The description of the floor that the printer is located on.</span></span>|
|<span data-ttu-id="fb4f8-149">roomName</span><span class="sxs-lookup"><span data-stu-id="fb4f8-149">roomName</span></span>|<span data-ttu-id="fb4f8-150">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fb4f8-150">String</span></span>|<span data-ttu-id="fb4f8-151">A sala em que a impressora está localizada.</span><span class="sxs-lookup"><span data-stu-id="fb4f8-151">The room that the printer is located in.</span></span> <span data-ttu-id="fb4f8-152">Somente valores numéricos são suportados no momento.</span><span class="sxs-lookup"><span data-stu-id="fb4f8-152">Only numerical values are supported right now.</span></span>|
|<span data-ttu-id="fb4f8-153">roomDescription</span><span class="sxs-lookup"><span data-stu-id="fb4f8-153">roomDescription</span></span>|<span data-ttu-id="fb4f8-154">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fb4f8-154">String</span></span>|<span data-ttu-id="fb4f8-155">A descrição da sala em que a impressora está localizada.</span><span class="sxs-lookup"><span data-stu-id="fb4f8-155">The description of the room that the printer is located in.</span></span>|
|<span data-ttu-id="fb4f8-156">organização</span><span class="sxs-lookup"><span data-stu-id="fb4f8-156">organization</span></span>|<span data-ttu-id="fb4f8-157">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="fb4f8-157">String collection</span></span>|<span data-ttu-id="fb4f8-158">A hierarquia organizacional à que a impressora pertence.</span><span class="sxs-lookup"><span data-stu-id="fb4f8-158">The organizational hierarchy that the printer belongs to.</span></span> <span data-ttu-id="fb4f8-159">Os elementos devem estar em ordem hierárquica.</span><span class="sxs-lookup"><span data-stu-id="fb4f8-159">The elements should be in hierarchical order.</span></span>|
|<span data-ttu-id="fb4f8-160">subdivisão</span><span class="sxs-lookup"><span data-stu-id="fb4f8-160">subdivision</span></span>|<span data-ttu-id="fb4f8-161">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="fb4f8-161">String collection</span></span>|<span data-ttu-id="fb4f8-162">A subdivisão em que a impressora está localizada.</span><span class="sxs-lookup"><span data-stu-id="fb4f8-162">The subdivision that the printer is located in.</span></span> <span data-ttu-id="fb4f8-163">Os elementos devem estar em ordem hierárquica.</span><span class="sxs-lookup"><span data-stu-id="fb4f8-163">The elements should be in hierarchical order.</span></span>|
|<span data-ttu-id="fb4f8-164">stateOrProvince</span><span class="sxs-lookup"><span data-stu-id="fb4f8-164">stateOrProvince</span></span>|<span data-ttu-id="fb4f8-165">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fb4f8-165">String</span></span>|<span data-ttu-id="fb4f8-166">O estado ou província em que a impressora está localizada.</span><span class="sxs-lookup"><span data-stu-id="fb4f8-166">The state or province that the printer is located in.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fb4f8-167">Relações</span><span class="sxs-lookup"><span data-stu-id="fb4f8-167">Relationships</span></span>
<span data-ttu-id="fb4f8-168">Nenhum</span><span class="sxs-lookup"><span data-stu-id="fb4f8-168">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="fb4f8-169">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fb4f8-169">JSON representation</span></span>
<span data-ttu-id="fb4f8-170">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="fb4f8-170">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.printerLocation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printerLocation",
  "latitude": "Double",
  "longitude": "Double",
  "altitudeInMeters": "Integer",
  "streetAddress": "String",
  "subunit": [
    "String"
  ],
  "city": "String",
  "postalCode": "String",
  "countryOrRegion": "String",
  "site": "String",
  "building": "String",
  "floor": "String",
  "floorDescription": "String",
  "roomName": "String",
  "roomDescription": "String",
  "organization": [
    "String"
  ],
  "subdivision": [
    "String"
  ],
  "stateOrProvince": "String"
}
```

