---
title: tipo de recurso Onpremisesextensionattributes à
description: A propriedade **onpremisesextensionattributes à** da entidade de usuário contém quinze Propriedades de atributos de extensões personalizadas. Para um usuário do **onPremisesSyncEnabled** , esse conjunto de propriedades é Mastered no Active Directory local e sincronizado com o Azure AD e é somente leitura. Para um usuário somente na nuvem (onde **onPremisesSyncEnabled** é false), essas propriedades podem ser definidas durante a criação ou atualização.
localization_priority: Normal
ms.openlocfilehash: 14e6d8530e67f40704d1052ef5e66cf9046b883f
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33341787"
---
# <a name="onpremisesextensionattributes-resource-type"></a><span data-ttu-id="9afef-105">tipo de recurso Onpremisesextensionattributes à</span><span class="sxs-lookup"><span data-stu-id="9afef-105">onPremisesExtensionAttributes resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9afef-106">A propriedade **onpremisesextensionattributes à** da entidade de [usuário](user.md) contém quinze Propriedades de atributos de extensões personalizadas.</span><span class="sxs-lookup"><span data-stu-id="9afef-106">The **onPremisesExtensionAttributes** property of the [user](user.md) entity contains fifteen custom extension attribute properties.</span></span> <span data-ttu-id="9afef-107">Para um usuário do **onPremisesSyncEnabled** , esse conjunto de propriedades é Mastered no Active Directory local e sincronizado com o Azure AD e é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9afef-107">For an **onPremisesSyncEnabled** user, this set of properties is mastered in on-premises Active Directory and synchronized to Azure AD, and is read-only.</span></span> <span data-ttu-id="9afef-108">Para um usuário somente na nuvem (onde **onPremisesSyncEnabled** é false), essas propriedades podem ser definidas durante a criação ou atualização.</span><span class="sxs-lookup"><span data-stu-id="9afef-108">For a cloud-only user (where **onPremisesSyncEnabled** is false), these properties may be set during creation or update.</span></span>


## <a name="properties"></a><span data-ttu-id="9afef-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9afef-109">Properties</span></span>
| <span data-ttu-id="9afef-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9afef-110">Property</span></span>     | <span data-ttu-id="9afef-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="9afef-111">Type</span></span>   |<span data-ttu-id="9afef-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="9afef-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9afef-113">extensionAttribute1</span><span class="sxs-lookup"><span data-stu-id="9afef-113">extensionAttribute1</span></span>|<span data-ttu-id="9afef-114">String</span><span class="sxs-lookup"><span data-stu-id="9afef-114">String</span></span>| <span data-ttu-id="9afef-115">Primeiro atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="9afef-115">First customizable extension attribute.</span></span> |
|<span data-ttu-id="9afef-116">extensionAttribute2</span><span class="sxs-lookup"><span data-stu-id="9afef-116">extensionAttribute2</span></span>|<span data-ttu-id="9afef-117">String</span><span class="sxs-lookup"><span data-stu-id="9afef-117">String</span></span>| <span data-ttu-id="9afef-118">Segundo atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="9afef-118">Second customizable extension attribute.</span></span> |
|<span data-ttu-id="9afef-119">extensionAttribute3</span><span class="sxs-lookup"><span data-stu-id="9afef-119">extensionAttribute3</span></span>|<span data-ttu-id="9afef-120">String</span><span class="sxs-lookup"><span data-stu-id="9afef-120">String</span></span>| <span data-ttu-id="9afef-121">Terceiro atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="9afef-121">Third customizable extension attribute.</span></span> |
|<span data-ttu-id="9afef-122">extensionAttribute4</span><span class="sxs-lookup"><span data-stu-id="9afef-122">extensionAttribute4</span></span>|<span data-ttu-id="9afef-123">String</span><span class="sxs-lookup"><span data-stu-id="9afef-123">String</span></span>| <span data-ttu-id="9afef-124">Quarto atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="9afef-124">Fourth customizable extension attribute.</span></span> |
|<span data-ttu-id="9afef-125">extensionAttribute5</span><span class="sxs-lookup"><span data-stu-id="9afef-125">extensionAttribute5</span></span>|<span data-ttu-id="9afef-126">String</span><span class="sxs-lookup"><span data-stu-id="9afef-126">String</span></span>| <span data-ttu-id="9afef-127">Quinto atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="9afef-127">Fifth customizable extension attribute.</span></span> |
|<span data-ttu-id="9afef-128">extensionAttribute6</span><span class="sxs-lookup"><span data-stu-id="9afef-128">extensionAttribute6</span></span>|<span data-ttu-id="9afef-129">String</span><span class="sxs-lookup"><span data-stu-id="9afef-129">String</span></span>| <span data-ttu-id="9afef-130">Sexto atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="9afef-130">Sixth customizable extension attribute.</span></span> |
|<span data-ttu-id="9afef-131">extensionAttribute7</span><span class="sxs-lookup"><span data-stu-id="9afef-131">extensionAttribute7</span></span>|<span data-ttu-id="9afef-132">String</span><span class="sxs-lookup"><span data-stu-id="9afef-132">String</span></span>| <span data-ttu-id="9afef-133">Sétimo atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="9afef-133">Seventh customizable extension attribute.</span></span> |
|<span data-ttu-id="9afef-134">extensionAttribute8</span><span class="sxs-lookup"><span data-stu-id="9afef-134">extensionAttribute8</span></span>|<span data-ttu-id="9afef-135">String</span><span class="sxs-lookup"><span data-stu-id="9afef-135">String</span></span>| <span data-ttu-id="9afef-136">Oitavo atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="9afef-136">Eighth customizable extension attribute.</span></span> |
|<span data-ttu-id="9afef-137">extensionAttribute9</span><span class="sxs-lookup"><span data-stu-id="9afef-137">extensionAttribute9</span></span>|<span data-ttu-id="9afef-138">String</span><span class="sxs-lookup"><span data-stu-id="9afef-138">String</span></span>| <span data-ttu-id="9afef-139">Nono atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="9afef-139">Ninth customizable extension attribute.</span></span> |
|<span data-ttu-id="9afef-140">extensionAttribute10</span><span class="sxs-lookup"><span data-stu-id="9afef-140">extensionAttribute10</span></span>|<span data-ttu-id="9afef-141">String</span><span class="sxs-lookup"><span data-stu-id="9afef-141">String</span></span>| <span data-ttu-id="9afef-142">Décimo atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="9afef-142">Tenth customizable extension attribute.</span></span> |
|<span data-ttu-id="9afef-143">extensionAttribute11</span><span class="sxs-lookup"><span data-stu-id="9afef-143">extensionAttribute11</span></span>|<span data-ttu-id="9afef-144">String</span><span class="sxs-lookup"><span data-stu-id="9afef-144">String</span></span>| <span data-ttu-id="9afef-145">Décimo primeiro atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="9afef-145">Eleventh customizable extension attribute.</span></span> |
|<span data-ttu-id="9afef-146">extensionAttribute12</span><span class="sxs-lookup"><span data-stu-id="9afef-146">extensionAttribute12</span></span>|<span data-ttu-id="9afef-147">String</span><span class="sxs-lookup"><span data-stu-id="9afef-147">String</span></span>| <span data-ttu-id="9afef-148">Décimo segundo atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="9afef-148">Twelfth customizable extension attribute.</span></span> |
|<span data-ttu-id="9afef-149">extensionAttribute13</span><span class="sxs-lookup"><span data-stu-id="9afef-149">extensionAttribute13</span></span>|<span data-ttu-id="9afef-150">String</span><span class="sxs-lookup"><span data-stu-id="9afef-150">String</span></span>| <span data-ttu-id="9afef-151">Décimo terceiro atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="9afef-151">Thirteenth customizable extension attribute.</span></span> |
|<span data-ttu-id="9afef-152">extensionAttribute14</span><span class="sxs-lookup"><span data-stu-id="9afef-152">extensionAttribute14</span></span>|<span data-ttu-id="9afef-153">String</span><span class="sxs-lookup"><span data-stu-id="9afef-153">String</span></span>| <span data-ttu-id="9afef-154">Atributo de extensão personalizável décimo quarto.</span><span class="sxs-lookup"><span data-stu-id="9afef-154">Fourteenth customizable extension attribute.</span></span> |
|<span data-ttu-id="9afef-155">extensionAttribute15</span><span class="sxs-lookup"><span data-stu-id="9afef-155">extensionAttribute15</span></span>|<span data-ttu-id="9afef-156">String</span><span class="sxs-lookup"><span data-stu-id="9afef-156">String</span></span>| <span data-ttu-id="9afef-157">Atributo de extensão personalizável décimo quinto.</span><span class="sxs-lookup"><span data-stu-id="9afef-157">Fifteenth customizable extension attribute.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="9afef-158">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9afef-158">JSON representation</span></span>

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
