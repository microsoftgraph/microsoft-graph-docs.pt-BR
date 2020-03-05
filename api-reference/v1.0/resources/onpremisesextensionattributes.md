---
title: tipo de recurso Onpremisesextensionattributes à
description: A propriedade **onpremisesextensionattributes à** da entidade de usuário contém quinze Propriedades de atributos de extensões personalizadas. Para um usuário do **onPremisesSyncEnabled** , esse conjunto de propriedades é Mastered no Active Directory local e sincronizado com o Azure AD e é somente leitura. Para um usuário somente na nuvem (onde **onPremisesSyncEnabled** é false), essas propriedades podem ser definidas durante a criação ou atualização.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: f6c80e5ee55409545f744556390a515125aee394
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447294"
---
# <a name="onpremisesextensionattributes-resource-type"></a><span data-ttu-id="3f519-105">tipo de recurso Onpremisesextensionattributes à</span><span class="sxs-lookup"><span data-stu-id="3f519-105">onPremisesExtensionAttributes resource type</span></span>

<span data-ttu-id="3f519-106">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="3f519-106">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3f519-107">A propriedade **onpremisesextensionattributes à** da entidade de [usuário](user.md) contém quinze Propriedades de atributos de extensões personalizadas.</span><span class="sxs-lookup"><span data-stu-id="3f519-107">The **onPremisesExtensionAttributes** property of the [user](user.md) entity contains fifteen custom extension attribute properties.</span></span> <span data-ttu-id="3f519-108">Para um usuário do **onPremisesSyncEnabled** , esse conjunto de propriedades é Mastered no Active Directory local e sincronizado com o Azure AD e é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3f519-108">For an **onPremisesSyncEnabled** user, this set of properties is mastered in on-premises Active Directory and synchronized to Azure AD, and is read-only.</span></span> <span data-ttu-id="3f519-109">Para um usuário somente na nuvem (onde **onPremisesSyncEnabled** é false), essas propriedades podem ser definidas durante a criação ou atualização.</span><span class="sxs-lookup"><span data-stu-id="3f519-109">For a cloud-only user (where **onPremisesSyncEnabled** is false), these properties may be set during creation or update.</span></span>


## <a name="properties"></a><span data-ttu-id="3f519-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3f519-110">Properties</span></span>
| <span data-ttu-id="3f519-111">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3f519-111">Property</span></span>     | <span data-ttu-id="3f519-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="3f519-112">Type</span></span>   |<span data-ttu-id="3f519-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="3f519-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3f519-114">extensionAttribute1</span><span class="sxs-lookup"><span data-stu-id="3f519-114">extensionAttribute1</span></span>|<span data-ttu-id="3f519-115">String</span><span class="sxs-lookup"><span data-stu-id="3f519-115">String</span></span>| <span data-ttu-id="3f519-116">Primeiro atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="3f519-116">First customizable extension attribute.</span></span> |
|<span data-ttu-id="3f519-117">extensionAttribute2</span><span class="sxs-lookup"><span data-stu-id="3f519-117">extensionAttribute2</span></span>|<span data-ttu-id="3f519-118">String</span><span class="sxs-lookup"><span data-stu-id="3f519-118">String</span></span>| <span data-ttu-id="3f519-119">Segundo atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="3f519-119">Second customizable extension attribute.</span></span> |
|<span data-ttu-id="3f519-120">extensionAttribute3</span><span class="sxs-lookup"><span data-stu-id="3f519-120">extensionAttribute3</span></span>|<span data-ttu-id="3f519-121">String</span><span class="sxs-lookup"><span data-stu-id="3f519-121">String</span></span>| <span data-ttu-id="3f519-122">Terceiro atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="3f519-122">Third customizable extension attribute.</span></span> |
|<span data-ttu-id="3f519-123">extensionAttribute4</span><span class="sxs-lookup"><span data-stu-id="3f519-123">extensionAttribute4</span></span>|<span data-ttu-id="3f519-124">String</span><span class="sxs-lookup"><span data-stu-id="3f519-124">String</span></span>| <span data-ttu-id="3f519-125">Quarto atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="3f519-125">Fourth customizable extension attribute.</span></span> |
|<span data-ttu-id="3f519-126">extensionAttribute5</span><span class="sxs-lookup"><span data-stu-id="3f519-126">extensionAttribute5</span></span>|<span data-ttu-id="3f519-127">String</span><span class="sxs-lookup"><span data-stu-id="3f519-127">String</span></span>| <span data-ttu-id="3f519-128">Quinto atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="3f519-128">Fifth customizable extension attribute.</span></span> |
|<span data-ttu-id="3f519-129">extensionAttribute6</span><span class="sxs-lookup"><span data-stu-id="3f519-129">extensionAttribute6</span></span>|<span data-ttu-id="3f519-130">String</span><span class="sxs-lookup"><span data-stu-id="3f519-130">String</span></span>| <span data-ttu-id="3f519-131">Sexto atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="3f519-131">Sixth customizable extension attribute.</span></span> |
|<span data-ttu-id="3f519-132">extensionAttribute7</span><span class="sxs-lookup"><span data-stu-id="3f519-132">extensionAttribute7</span></span>|<span data-ttu-id="3f519-133">String</span><span class="sxs-lookup"><span data-stu-id="3f519-133">String</span></span>| <span data-ttu-id="3f519-134">Sétimo atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="3f519-134">Seventh customizable extension attribute.</span></span> |
|<span data-ttu-id="3f519-135">extensionAttribute8</span><span class="sxs-lookup"><span data-stu-id="3f519-135">extensionAttribute8</span></span>|<span data-ttu-id="3f519-136">String</span><span class="sxs-lookup"><span data-stu-id="3f519-136">String</span></span>| <span data-ttu-id="3f519-137">Oitavo atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="3f519-137">Eighth customizable extension attribute.</span></span> |
|<span data-ttu-id="3f519-138">extensionAttribute9</span><span class="sxs-lookup"><span data-stu-id="3f519-138">extensionAttribute9</span></span>|<span data-ttu-id="3f519-139">String</span><span class="sxs-lookup"><span data-stu-id="3f519-139">String</span></span>| <span data-ttu-id="3f519-140">Nono atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="3f519-140">Ninth customizable extension attribute.</span></span> |
|<span data-ttu-id="3f519-141">extensionAttribute10</span><span class="sxs-lookup"><span data-stu-id="3f519-141">extensionAttribute10</span></span>|<span data-ttu-id="3f519-142">String</span><span class="sxs-lookup"><span data-stu-id="3f519-142">String</span></span>| <span data-ttu-id="3f519-143">Décimo atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="3f519-143">Tenth customizable extension attribute.</span></span> |
|<span data-ttu-id="3f519-144">extensionAttribute11</span><span class="sxs-lookup"><span data-stu-id="3f519-144">extensionAttribute11</span></span>|<span data-ttu-id="3f519-145">String</span><span class="sxs-lookup"><span data-stu-id="3f519-145">String</span></span>| <span data-ttu-id="3f519-146">Décimo primeiro atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="3f519-146">Eleventh customizable extension attribute.</span></span> |
|<span data-ttu-id="3f519-147">extensionAttribute12</span><span class="sxs-lookup"><span data-stu-id="3f519-147">extensionAttribute12</span></span>|<span data-ttu-id="3f519-148">String</span><span class="sxs-lookup"><span data-stu-id="3f519-148">String</span></span>| <span data-ttu-id="3f519-149">Décimo segundo atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="3f519-149">Twelfth customizable extension attribute.</span></span> |
|<span data-ttu-id="3f519-150">extensionAttribute13</span><span class="sxs-lookup"><span data-stu-id="3f519-150">extensionAttribute13</span></span>|<span data-ttu-id="3f519-151">String</span><span class="sxs-lookup"><span data-stu-id="3f519-151">String</span></span>| <span data-ttu-id="3f519-152">Décimo terceiro atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="3f519-152">Thirteenth customizable extension attribute.</span></span> |
|<span data-ttu-id="3f519-153">extensionAttribute14</span><span class="sxs-lookup"><span data-stu-id="3f519-153">extensionAttribute14</span></span>|<span data-ttu-id="3f519-154">String</span><span class="sxs-lookup"><span data-stu-id="3f519-154">String</span></span>| <span data-ttu-id="3f519-155">Atributo de extensão personalizável décimo quarto.</span><span class="sxs-lookup"><span data-stu-id="3f519-155">Fourteenth customizable extension attribute.</span></span> |
|<span data-ttu-id="3f519-156">extensionAttribute15</span><span class="sxs-lookup"><span data-stu-id="3f519-156">extensionAttribute15</span></span>|<span data-ttu-id="3f519-157">String</span><span class="sxs-lookup"><span data-stu-id="3f519-157">String</span></span>| <span data-ttu-id="3f519-158">Atributo de extensão personalizável décimo quinto.</span><span class="sxs-lookup"><span data-stu-id="3f519-158">Fifteenth customizable extension attribute.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="3f519-159">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3f519-159">JSON representation</span></span>

<span data-ttu-id="3f519-160">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="3f519-160">Here is a JSON representation of the resource</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "onPremisesExtensionAttributes resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
