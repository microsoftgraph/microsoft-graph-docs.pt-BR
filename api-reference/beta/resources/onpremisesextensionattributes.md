---
title: tipo de recurso Onpremisesextensionattributes à
description: A propriedade **onpremisesextensionattributes à** da entidade de usuário contém quinze Propriedades de atributos de extensões personalizadas. Para um usuário do **onPremisesSyncEnabled** , esse conjunto de propriedades é Mastered no Active Directory local e sincronizado com o Azure AD e é somente leitura. Para um usuário somente na nuvem (onde **onPremisesSyncEnabled** é false), essas propriedades podem ser definidas durante a criação ou atualização.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: cbcb3d548a99d33e05768c765ab7a7e06981acc0
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966395"
---
# <a name="onpremisesextensionattributes-resource-type"></a><span data-ttu-id="11d52-105">tipo de recurso Onpremisesextensionattributes à</span><span class="sxs-lookup"><span data-stu-id="11d52-105">onPremisesExtensionAttributes resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="11d52-106">A propriedade **onpremisesextensionattributes à** da entidade de [usuário](user.md) contém quinze Propriedades de atributos de extensões personalizadas.</span><span class="sxs-lookup"><span data-stu-id="11d52-106">The **onPremisesExtensionAttributes** property of the [user](user.md) entity contains fifteen custom extension attribute properties.</span></span> <span data-ttu-id="11d52-107">Para um usuário do **onPremisesSyncEnabled** , esse conjunto de propriedades é Mastered no Active Directory local e sincronizado com o Azure AD e é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="11d52-107">For an **onPremisesSyncEnabled** user, this set of properties is mastered in on-premises Active Directory and synchronized to Azure AD, and is read-only.</span></span> <span data-ttu-id="11d52-108">Para um usuário somente na nuvem (onde **onPremisesSyncEnabled** é false), essas propriedades podem ser definidas durante a criação ou atualização.</span><span class="sxs-lookup"><span data-stu-id="11d52-108">For a cloud-only user (where **onPremisesSyncEnabled** is false), these properties may be set during creation or update.</span></span>


## <a name="properties"></a><span data-ttu-id="11d52-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="11d52-109">Properties</span></span>
| <span data-ttu-id="11d52-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="11d52-110">Property</span></span>     | <span data-ttu-id="11d52-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="11d52-111">Type</span></span>   |<span data-ttu-id="11d52-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="11d52-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="11d52-113">extensionAttribute1</span><span class="sxs-lookup"><span data-stu-id="11d52-113">extensionAttribute1</span></span>|<span data-ttu-id="11d52-114">String</span><span class="sxs-lookup"><span data-stu-id="11d52-114">String</span></span>| <span data-ttu-id="11d52-115">Primeiro atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="11d52-115">First customizable extension attribute.</span></span> |
|<span data-ttu-id="11d52-116">extensionAttribute2</span><span class="sxs-lookup"><span data-stu-id="11d52-116">extensionAttribute2</span></span>|<span data-ttu-id="11d52-117">String</span><span class="sxs-lookup"><span data-stu-id="11d52-117">String</span></span>| <span data-ttu-id="11d52-118">Segundo atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="11d52-118">Second customizable extension attribute.</span></span> |
|<span data-ttu-id="11d52-119">extensionAttribute3</span><span class="sxs-lookup"><span data-stu-id="11d52-119">extensionAttribute3</span></span>|<span data-ttu-id="11d52-120">String</span><span class="sxs-lookup"><span data-stu-id="11d52-120">String</span></span>| <span data-ttu-id="11d52-121">Terceiro atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="11d52-121">Third customizable extension attribute.</span></span> |
|<span data-ttu-id="11d52-122">extensionAttribute4</span><span class="sxs-lookup"><span data-stu-id="11d52-122">extensionAttribute4</span></span>|<span data-ttu-id="11d52-123">String</span><span class="sxs-lookup"><span data-stu-id="11d52-123">String</span></span>| <span data-ttu-id="11d52-124">Quarto atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="11d52-124">Fourth customizable extension attribute.</span></span> |
|<span data-ttu-id="11d52-125">extensionAttribute5</span><span class="sxs-lookup"><span data-stu-id="11d52-125">extensionAttribute5</span></span>|<span data-ttu-id="11d52-126">String</span><span class="sxs-lookup"><span data-stu-id="11d52-126">String</span></span>| <span data-ttu-id="11d52-127">Quinto atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="11d52-127">Fifth customizable extension attribute.</span></span> |
|<span data-ttu-id="11d52-128">extensionAttribute6</span><span class="sxs-lookup"><span data-stu-id="11d52-128">extensionAttribute6</span></span>|<span data-ttu-id="11d52-129">String</span><span class="sxs-lookup"><span data-stu-id="11d52-129">String</span></span>| <span data-ttu-id="11d52-130">Sexto atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="11d52-130">Sixth customizable extension attribute.</span></span> |
|<span data-ttu-id="11d52-131">extensionAttribute7</span><span class="sxs-lookup"><span data-stu-id="11d52-131">extensionAttribute7</span></span>|<span data-ttu-id="11d52-132">String</span><span class="sxs-lookup"><span data-stu-id="11d52-132">String</span></span>| <span data-ttu-id="11d52-133">Sétimo atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="11d52-133">Seventh customizable extension attribute.</span></span> |
|<span data-ttu-id="11d52-134">extensionAttribute8</span><span class="sxs-lookup"><span data-stu-id="11d52-134">extensionAttribute8</span></span>|<span data-ttu-id="11d52-135">String</span><span class="sxs-lookup"><span data-stu-id="11d52-135">String</span></span>| <span data-ttu-id="11d52-136">Oitavo atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="11d52-136">Eighth customizable extension attribute.</span></span> |
|<span data-ttu-id="11d52-137">extensionAttribute9</span><span class="sxs-lookup"><span data-stu-id="11d52-137">extensionAttribute9</span></span>|<span data-ttu-id="11d52-138">String</span><span class="sxs-lookup"><span data-stu-id="11d52-138">String</span></span>| <span data-ttu-id="11d52-139">Nono atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="11d52-139">Ninth customizable extension attribute.</span></span> |
|<span data-ttu-id="11d52-140">extensionAttribute10</span><span class="sxs-lookup"><span data-stu-id="11d52-140">extensionAttribute10</span></span>|<span data-ttu-id="11d52-141">String</span><span class="sxs-lookup"><span data-stu-id="11d52-141">String</span></span>| <span data-ttu-id="11d52-142">Décimo atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="11d52-142">Tenth customizable extension attribute.</span></span> |
|<span data-ttu-id="11d52-143">extensionAttribute11</span><span class="sxs-lookup"><span data-stu-id="11d52-143">extensionAttribute11</span></span>|<span data-ttu-id="11d52-144">String</span><span class="sxs-lookup"><span data-stu-id="11d52-144">String</span></span>| <span data-ttu-id="11d52-145">Décimo primeiro atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="11d52-145">Eleventh customizable extension attribute.</span></span> |
|<span data-ttu-id="11d52-146">extensionAttribute12</span><span class="sxs-lookup"><span data-stu-id="11d52-146">extensionAttribute12</span></span>|<span data-ttu-id="11d52-147">String</span><span class="sxs-lookup"><span data-stu-id="11d52-147">String</span></span>| <span data-ttu-id="11d52-148">Décimo segundo atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="11d52-148">Twelfth customizable extension attribute.</span></span> |
|<span data-ttu-id="11d52-149">extensionAttribute13</span><span class="sxs-lookup"><span data-stu-id="11d52-149">extensionAttribute13</span></span>|<span data-ttu-id="11d52-150">String</span><span class="sxs-lookup"><span data-stu-id="11d52-150">String</span></span>| <span data-ttu-id="11d52-151">Décimo terceiro atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="11d52-151">Thirteenth customizable extension attribute.</span></span> |
|<span data-ttu-id="11d52-152">extensionAttribute14</span><span class="sxs-lookup"><span data-stu-id="11d52-152">extensionAttribute14</span></span>|<span data-ttu-id="11d52-153">String</span><span class="sxs-lookup"><span data-stu-id="11d52-153">String</span></span>| <span data-ttu-id="11d52-154">Atributo de extensão personalizável décimo quarto.</span><span class="sxs-lookup"><span data-stu-id="11d52-154">Fourteenth customizable extension attribute.</span></span> |
|<span data-ttu-id="11d52-155">extensionAttribute15</span><span class="sxs-lookup"><span data-stu-id="11d52-155">extensionAttribute15</span></span>|<span data-ttu-id="11d52-156">String</span><span class="sxs-lookup"><span data-stu-id="11d52-156">String</span></span>| <span data-ttu-id="11d52-157">Atributo de extensão personalizável décimo quinto.</span><span class="sxs-lookup"><span data-stu-id="11d52-157">Fifteenth customizable extension attribute.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="11d52-158">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="11d52-158">JSON representation</span></span>

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
