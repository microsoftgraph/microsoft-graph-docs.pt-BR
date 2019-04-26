---
title: tipo de recurso Onpremisesextensionattributes à
description: A propriedade **onpremisesextensionattributes à** da entidade de usuário contém quinze Propriedades de atributos de extensões personalizadas. Para um usuário do **onPremisesSyncEnabled** , esse conjunto de propriedades é Mastered no Active Directory local e sincronizado com o Azure AD e é somente leitura. Para um usuário somente na nuvem (onde **onPremisesSyncEnabled** é false), essas propriedades podem ser definidas durante a criação ou atualização.
localization_priority: Normal
ms.openlocfilehash: f44f71fdcd86d2165289282568a2d7153ccc99b1
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32568875"
---
# <a name="onpremisesextensionattributes-resource-type"></a><span data-ttu-id="c68c5-105">tipo de recurso Onpremisesextensionattributes à</span><span class="sxs-lookup"><span data-stu-id="c68c5-105">onPremisesExtensionAttributes resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c68c5-106">A propriedade **onpremisesextensionattributes à** da entidade de [usuário](user.md) contém quinze Propriedades de atributos de extensões personalizadas.</span><span class="sxs-lookup"><span data-stu-id="c68c5-106">The **onPremisesExtensionAttributes** property of the [user](user.md) entity contains fifteen custom extension attribute properties.</span></span> <span data-ttu-id="c68c5-107">Para um usuário do **onPremisesSyncEnabled** , esse conjunto de propriedades é Mastered no Active Directory local e sincronizado com o Azure AD e é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c68c5-107">For an **onPremisesSyncEnabled** user, this set of properties is mastered in on-premises Active Directory and synchronized to Azure AD, and is read-only.</span></span> <span data-ttu-id="c68c5-108">Para um usuário somente na nuvem (onde **onPremisesSyncEnabled** é false), essas propriedades podem ser definidas durante a criação ou atualização.</span><span class="sxs-lookup"><span data-stu-id="c68c5-108">For a cloud-only user (where **onPremisesSyncEnabled** is false), these properties may be set during creation or update.</span></span>


## <a name="properties"></a><span data-ttu-id="c68c5-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c68c5-109">Properties</span></span>
| <span data-ttu-id="c68c5-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c68c5-110">Property</span></span>     | <span data-ttu-id="c68c5-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="c68c5-111">Type</span></span>   |<span data-ttu-id="c68c5-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="c68c5-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c68c5-113">extensionAttribute1</span><span class="sxs-lookup"><span data-stu-id="c68c5-113">extensionAttribute1</span></span>|<span data-ttu-id="c68c5-114">String</span><span class="sxs-lookup"><span data-stu-id="c68c5-114">String</span></span>| <span data-ttu-id="c68c5-115">Primeiro atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="c68c5-115">First customizable extension attribute.</span></span> |
|<span data-ttu-id="c68c5-116">extensionAttribute2</span><span class="sxs-lookup"><span data-stu-id="c68c5-116">extensionAttribute2</span></span>|<span data-ttu-id="c68c5-117">String</span><span class="sxs-lookup"><span data-stu-id="c68c5-117">String</span></span>| <span data-ttu-id="c68c5-118">Segundo atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="c68c5-118">Second customizable extension attribute.</span></span> |
|<span data-ttu-id="c68c5-119">extensionAttribute3</span><span class="sxs-lookup"><span data-stu-id="c68c5-119">extensionAttribute3</span></span>|<span data-ttu-id="c68c5-120">String</span><span class="sxs-lookup"><span data-stu-id="c68c5-120">String</span></span>| <span data-ttu-id="c68c5-121">Terceiro atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="c68c5-121">Third customizable extension attribute.</span></span> |
|<span data-ttu-id="c68c5-122">extensionAttribute4</span><span class="sxs-lookup"><span data-stu-id="c68c5-122">extensionAttribute4</span></span>|<span data-ttu-id="c68c5-123">String</span><span class="sxs-lookup"><span data-stu-id="c68c5-123">String</span></span>| <span data-ttu-id="c68c5-124">Quarto atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="c68c5-124">Fourth customizable extension attribute.</span></span> |
|<span data-ttu-id="c68c5-125">extensionAttribute5</span><span class="sxs-lookup"><span data-stu-id="c68c5-125">extensionAttribute5</span></span>|<span data-ttu-id="c68c5-126">String</span><span class="sxs-lookup"><span data-stu-id="c68c5-126">String</span></span>| <span data-ttu-id="c68c5-127">Quinto atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="c68c5-127">Fifth customizable extension attribute.</span></span> |
|<span data-ttu-id="c68c5-128">extensionAttribute6</span><span class="sxs-lookup"><span data-stu-id="c68c5-128">extensionAttribute6</span></span>|<span data-ttu-id="c68c5-129">String</span><span class="sxs-lookup"><span data-stu-id="c68c5-129">String</span></span>| <span data-ttu-id="c68c5-130">Sexto atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="c68c5-130">Sixth customizable extension attribute.</span></span> |
|<span data-ttu-id="c68c5-131">extensionAttribute7</span><span class="sxs-lookup"><span data-stu-id="c68c5-131">extensionAttribute7</span></span>|<span data-ttu-id="c68c5-132">String</span><span class="sxs-lookup"><span data-stu-id="c68c5-132">String</span></span>| <span data-ttu-id="c68c5-133">Sétimo atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="c68c5-133">Seventh customizable extension attribute.</span></span> |
|<span data-ttu-id="c68c5-134">extensionAttribute8</span><span class="sxs-lookup"><span data-stu-id="c68c5-134">extensionAttribute8</span></span>|<span data-ttu-id="c68c5-135">String</span><span class="sxs-lookup"><span data-stu-id="c68c5-135">String</span></span>| <span data-ttu-id="c68c5-136">Oitavo atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="c68c5-136">Eighth customizable extension attribute.</span></span> |
|<span data-ttu-id="c68c5-137">extensionAttribute9</span><span class="sxs-lookup"><span data-stu-id="c68c5-137">extensionAttribute9</span></span>|<span data-ttu-id="c68c5-138">String</span><span class="sxs-lookup"><span data-stu-id="c68c5-138">String</span></span>| <span data-ttu-id="c68c5-139">Nono atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="c68c5-139">Ninth customizable extension attribute.</span></span> |
|<span data-ttu-id="c68c5-140">extensionAttribute10</span><span class="sxs-lookup"><span data-stu-id="c68c5-140">extensionAttribute10</span></span>|<span data-ttu-id="c68c5-141">String</span><span class="sxs-lookup"><span data-stu-id="c68c5-141">String</span></span>| <span data-ttu-id="c68c5-142">Décimo atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="c68c5-142">Tenth customizable extension attribute.</span></span> |
|<span data-ttu-id="c68c5-143">extensionAttribute11</span><span class="sxs-lookup"><span data-stu-id="c68c5-143">extensionAttribute11</span></span>|<span data-ttu-id="c68c5-144">String</span><span class="sxs-lookup"><span data-stu-id="c68c5-144">String</span></span>| <span data-ttu-id="c68c5-145">Décimo primeiro atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="c68c5-145">Eleventh customizable extension attribute.</span></span> |
|<span data-ttu-id="c68c5-146">extensionAttribute12</span><span class="sxs-lookup"><span data-stu-id="c68c5-146">extensionAttribute12</span></span>|<span data-ttu-id="c68c5-147">String</span><span class="sxs-lookup"><span data-stu-id="c68c5-147">String</span></span>| <span data-ttu-id="c68c5-148">Décimo segundo atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="c68c5-148">Twelfth customizable extension attribute.</span></span> |
|<span data-ttu-id="c68c5-149">extensionAttribute13</span><span class="sxs-lookup"><span data-stu-id="c68c5-149">extensionAttribute13</span></span>|<span data-ttu-id="c68c5-150">String</span><span class="sxs-lookup"><span data-stu-id="c68c5-150">String</span></span>| <span data-ttu-id="c68c5-151">Décimo terceiro atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="c68c5-151">Thirteenth customizable extension attribute.</span></span> |
|<span data-ttu-id="c68c5-152">extensionAttribute14</span><span class="sxs-lookup"><span data-stu-id="c68c5-152">extensionAttribute14</span></span>|<span data-ttu-id="c68c5-153">String</span><span class="sxs-lookup"><span data-stu-id="c68c5-153">String</span></span>| <span data-ttu-id="c68c5-154">Atributo de extensão personalizável décimo quarto.</span><span class="sxs-lookup"><span data-stu-id="c68c5-154">Fourteenth customizable extension attribute.</span></span> |
|<span data-ttu-id="c68c5-155">extensionAttribute15</span><span class="sxs-lookup"><span data-stu-id="c68c5-155">extensionAttribute15</span></span>|<span data-ttu-id="c68c5-156">String</span><span class="sxs-lookup"><span data-stu-id="c68c5-156">String</span></span>| <span data-ttu-id="c68c5-157">Atributo de extensão personalizável décimo quinto.</span><span class="sxs-lookup"><span data-stu-id="c68c5-157">Fifteenth customizable extension attribute.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="c68c5-158">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c68c5-158">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onPremisesExtensionAttributes"
}-->


```json
{
      "extensionAttribute1": "string",
      "extensionAttribute2": "string",
      "extensionAttribute3": "string",
      "extensionAttribute4": "string",
      "extensionAttribute5": "string",
      "extensionAttribute6": "string",
      "extensionAttribute7": "string",
      "extensionAttribute8": "string",
      "extensionAttribute9": "string",
      "extensionAttribute10": "string",
      "extensionAttribute11": "string",
      "extensionAttribute12": "string",
      "extensionAttribute13": "string",
      "extensionAttribute14": "string",
      "extensionAttribute15": "string"
  }

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "onPremisesExtensionAttributes resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
