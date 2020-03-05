---
title: tipo de recurso Onpremisesextensionattributes à
description: A propriedade **onpremisesextensionattributes à** da entidade de usuário contém quinze Propriedades de atributos de extensões personalizadas. Para um usuário do **onPremisesSyncEnabled** , esse conjunto de propriedades é Mastered no Active Directory local e sincronizado com o Azure AD e é somente leitura. Para um usuário somente na nuvem (onde **onPremisesSyncEnabled** é false), essas propriedades podem ser definidas durante a criação ou atualização.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 809f299e97fc3341b822a7223d3e6fcb196efc33
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522225"
---
# <a name="onpremisesextensionattributes-resource-type"></a><span data-ttu-id="ba867-105">tipo de recurso Onpremisesextensionattributes à</span><span class="sxs-lookup"><span data-stu-id="ba867-105">onPremisesExtensionAttributes resource type</span></span>

<span data-ttu-id="ba867-106">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="ba867-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ba867-107">A propriedade **onpremisesextensionattributes à** da entidade de [usuário](user.md) contém quinze Propriedades de atributos de extensões personalizadas.</span><span class="sxs-lookup"><span data-stu-id="ba867-107">The **onPremisesExtensionAttributes** property of the [user](user.md) entity contains fifteen custom extension attribute properties.</span></span> <span data-ttu-id="ba867-108">Para um usuário do **onPremisesSyncEnabled** , esse conjunto de propriedades é Mastered no Active Directory local e sincronizado com o Azure AD e é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ba867-108">For an **onPremisesSyncEnabled** user, this set of properties is mastered in on-premises Active Directory and synchronized to Azure AD, and is read-only.</span></span> <span data-ttu-id="ba867-109">Para um usuário somente na nuvem (onde **onPremisesSyncEnabled** é false), essas propriedades podem ser definidas durante a criação ou atualização.</span><span class="sxs-lookup"><span data-stu-id="ba867-109">For a cloud-only user (where **onPremisesSyncEnabled** is false), these properties may be set during creation or update.</span></span>


## <a name="properties"></a><span data-ttu-id="ba867-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ba867-110">Properties</span></span>
| <span data-ttu-id="ba867-111">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ba867-111">Property</span></span>     | <span data-ttu-id="ba867-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="ba867-112">Type</span></span>   |<span data-ttu-id="ba867-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="ba867-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ba867-114">extensionAttribute1</span><span class="sxs-lookup"><span data-stu-id="ba867-114">extensionAttribute1</span></span>|<span data-ttu-id="ba867-115">String</span><span class="sxs-lookup"><span data-stu-id="ba867-115">String</span></span>| <span data-ttu-id="ba867-116">Primeiro atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="ba867-116">First customizable extension attribute.</span></span> |
|<span data-ttu-id="ba867-117">extensionAttribute2</span><span class="sxs-lookup"><span data-stu-id="ba867-117">extensionAttribute2</span></span>|<span data-ttu-id="ba867-118">String</span><span class="sxs-lookup"><span data-stu-id="ba867-118">String</span></span>| <span data-ttu-id="ba867-119">Segundo atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="ba867-119">Second customizable extension attribute.</span></span> |
|<span data-ttu-id="ba867-120">extensionAttribute3</span><span class="sxs-lookup"><span data-stu-id="ba867-120">extensionAttribute3</span></span>|<span data-ttu-id="ba867-121">String</span><span class="sxs-lookup"><span data-stu-id="ba867-121">String</span></span>| <span data-ttu-id="ba867-122">Terceiro atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="ba867-122">Third customizable extension attribute.</span></span> |
|<span data-ttu-id="ba867-123">extensionAttribute4</span><span class="sxs-lookup"><span data-stu-id="ba867-123">extensionAttribute4</span></span>|<span data-ttu-id="ba867-124">String</span><span class="sxs-lookup"><span data-stu-id="ba867-124">String</span></span>| <span data-ttu-id="ba867-125">Quarto atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="ba867-125">Fourth customizable extension attribute.</span></span> |
|<span data-ttu-id="ba867-126">extensionAttribute5</span><span class="sxs-lookup"><span data-stu-id="ba867-126">extensionAttribute5</span></span>|<span data-ttu-id="ba867-127">String</span><span class="sxs-lookup"><span data-stu-id="ba867-127">String</span></span>| <span data-ttu-id="ba867-128">Quinto atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="ba867-128">Fifth customizable extension attribute.</span></span> |
|<span data-ttu-id="ba867-129">extensionAttribute6</span><span class="sxs-lookup"><span data-stu-id="ba867-129">extensionAttribute6</span></span>|<span data-ttu-id="ba867-130">String</span><span class="sxs-lookup"><span data-stu-id="ba867-130">String</span></span>| <span data-ttu-id="ba867-131">Sexto atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="ba867-131">Sixth customizable extension attribute.</span></span> |
|<span data-ttu-id="ba867-132">extensionAttribute7</span><span class="sxs-lookup"><span data-stu-id="ba867-132">extensionAttribute7</span></span>|<span data-ttu-id="ba867-133">String</span><span class="sxs-lookup"><span data-stu-id="ba867-133">String</span></span>| <span data-ttu-id="ba867-134">Sétimo atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="ba867-134">Seventh customizable extension attribute.</span></span> |
|<span data-ttu-id="ba867-135">extensionAttribute8</span><span class="sxs-lookup"><span data-stu-id="ba867-135">extensionAttribute8</span></span>|<span data-ttu-id="ba867-136">String</span><span class="sxs-lookup"><span data-stu-id="ba867-136">String</span></span>| <span data-ttu-id="ba867-137">Oitavo atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="ba867-137">Eighth customizable extension attribute.</span></span> |
|<span data-ttu-id="ba867-138">extensionAttribute9</span><span class="sxs-lookup"><span data-stu-id="ba867-138">extensionAttribute9</span></span>|<span data-ttu-id="ba867-139">String</span><span class="sxs-lookup"><span data-stu-id="ba867-139">String</span></span>| <span data-ttu-id="ba867-140">Nono atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="ba867-140">Ninth customizable extension attribute.</span></span> |
|<span data-ttu-id="ba867-141">extensionAttribute10</span><span class="sxs-lookup"><span data-stu-id="ba867-141">extensionAttribute10</span></span>|<span data-ttu-id="ba867-142">String</span><span class="sxs-lookup"><span data-stu-id="ba867-142">String</span></span>| <span data-ttu-id="ba867-143">Décimo atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="ba867-143">Tenth customizable extension attribute.</span></span> |
|<span data-ttu-id="ba867-144">extensionAttribute11</span><span class="sxs-lookup"><span data-stu-id="ba867-144">extensionAttribute11</span></span>|<span data-ttu-id="ba867-145">String</span><span class="sxs-lookup"><span data-stu-id="ba867-145">String</span></span>| <span data-ttu-id="ba867-146">Décimo primeiro atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="ba867-146">Eleventh customizable extension attribute.</span></span> |
|<span data-ttu-id="ba867-147">extensionAttribute12</span><span class="sxs-lookup"><span data-stu-id="ba867-147">extensionAttribute12</span></span>|<span data-ttu-id="ba867-148">String</span><span class="sxs-lookup"><span data-stu-id="ba867-148">String</span></span>| <span data-ttu-id="ba867-149">Décimo segundo atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="ba867-149">Twelfth customizable extension attribute.</span></span> |
|<span data-ttu-id="ba867-150">extensionAttribute13</span><span class="sxs-lookup"><span data-stu-id="ba867-150">extensionAttribute13</span></span>|<span data-ttu-id="ba867-151">String</span><span class="sxs-lookup"><span data-stu-id="ba867-151">String</span></span>| <span data-ttu-id="ba867-152">Décimo terceiro atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="ba867-152">Thirteenth customizable extension attribute.</span></span> |
|<span data-ttu-id="ba867-153">extensionAttribute14</span><span class="sxs-lookup"><span data-stu-id="ba867-153">extensionAttribute14</span></span>|<span data-ttu-id="ba867-154">String</span><span class="sxs-lookup"><span data-stu-id="ba867-154">String</span></span>| <span data-ttu-id="ba867-155">Atributo de extensão personalizável décimo quarto.</span><span class="sxs-lookup"><span data-stu-id="ba867-155">Fourteenth customizable extension attribute.</span></span> |
|<span data-ttu-id="ba867-156">extensionAttribute15</span><span class="sxs-lookup"><span data-stu-id="ba867-156">extensionAttribute15</span></span>|<span data-ttu-id="ba867-157">String</span><span class="sxs-lookup"><span data-stu-id="ba867-157">String</span></span>| <span data-ttu-id="ba867-158">Atributo de extensão personalizável décimo quinto.</span><span class="sxs-lookup"><span data-stu-id="ba867-158">Fifteenth customizable extension attribute.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="ba867-159">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ba867-159">JSON representation</span></span>

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
