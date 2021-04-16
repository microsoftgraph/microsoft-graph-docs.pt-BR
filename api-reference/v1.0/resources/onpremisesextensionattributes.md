---
title: Tipo de recurso onPremisesExtensionAttributes
description: A **propriedade onPremisesExtensionAttributes** da entidade do usuário contém quinze propriedades de atributo de extensão personalizadas. Para um usuário **onPremisesSyncEnabled,** esse conjunto de propriedades é mestre no Active Directory local e sincronizado com o Azure AD, e é somente leitura. Para um usuário somente na nuvem (onde **onPremisesSyncEnabled** é false), essas propriedades podem ser definidas sobre o Exchange Online. Os atributos são lidos somente no Microsoft Graph.
localization_priority: Normal
author: jpettere
ms.prod: users
doc_type: resourcePageType
ms.openlocfilehash: f21369156e1a1337d16d64be40bd6de210bd56d2
ms.sourcegitcommit: 412507a3c3a8e407fcc43b7cd227d4db35791f58
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2021
ms.locfileid: "51766102"
---
# <a name="onpremisesextensionattributes-resource-type"></a><span data-ttu-id="44084-106">Tipo de recurso onPremisesExtensionAttributes</span><span class="sxs-lookup"><span data-stu-id="44084-106">onPremisesExtensionAttributes resource type</span></span>

<span data-ttu-id="44084-107">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="44084-107">Namespace: microsoft.graph</span></span>

<span data-ttu-id="44084-108">A **propriedade onPremisesExtensionAttributes** da entidade do usuário contém quinze propriedades de atributo de extensão personalizadas. [](user.md)</span><span class="sxs-lookup"><span data-stu-id="44084-108">The **onPremisesExtensionAttributes** property of the [user](user.md) entity contains fifteen custom extension attribute properties.</span></span> <span data-ttu-id="44084-109">Para um usuário **onPremisesSyncEnabled,** a fonte de autoridade para esse conjunto de propriedades é o Active Directory local que é sincronizado com o Azure AD e é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="44084-109">For an **onPremisesSyncEnabled** user, the source of authority for this set of properties is the on-premises Active Directory which is synchronized to Azure AD, and is read-only.</span></span> <span data-ttu-id="44084-110">Para um usuário somente na nuvem (onde **onPremisesSyncEnabled** é false), essas propriedades podem ser definidas sobre o Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="44084-110">For a cloud-only user (where **onPremisesSyncEnabled** is false), these properties can be set over Exchange Online.</span></span> <span data-ttu-id="44084-111">Os atributos são lidos somente no Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="44084-111">The attributes are read only in Microsoft Graph.</span></span>

> <span data-ttu-id="44084-112">**Observação:** Esses atributos de extensão também são conhecidos como atributos personalizados do Exchange 1-15.</span><span class="sxs-lookup"><span data-stu-id="44084-112">**Note:** These extension attributes are also known as Exchange custom attributes 1-15.</span></span>

## <a name="properties"></a><span data-ttu-id="44084-113">Propriedades</span><span class="sxs-lookup"><span data-stu-id="44084-113">Properties</span></span>
| <span data-ttu-id="44084-114">Propriedade</span><span class="sxs-lookup"><span data-stu-id="44084-114">Property</span></span>     | <span data-ttu-id="44084-115">Tipo</span><span class="sxs-lookup"><span data-stu-id="44084-115">Type</span></span>   |<span data-ttu-id="44084-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="44084-116">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="44084-117">extensionAttribute1</span><span class="sxs-lookup"><span data-stu-id="44084-117">extensionAttribute1</span></span>|<span data-ttu-id="44084-118">String</span><span class="sxs-lookup"><span data-stu-id="44084-118">String</span></span>| <span data-ttu-id="44084-119">Primeiro atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="44084-119">First customizable extension attribute.</span></span> |
|<span data-ttu-id="44084-120">extensionAttribute2</span><span class="sxs-lookup"><span data-stu-id="44084-120">extensionAttribute2</span></span>|<span data-ttu-id="44084-121">String</span><span class="sxs-lookup"><span data-stu-id="44084-121">String</span></span>| <span data-ttu-id="44084-122">Segundo atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="44084-122">Second customizable extension attribute.</span></span> |
|<span data-ttu-id="44084-123">extensionAttribute3</span><span class="sxs-lookup"><span data-stu-id="44084-123">extensionAttribute3</span></span>|<span data-ttu-id="44084-124">String</span><span class="sxs-lookup"><span data-stu-id="44084-124">String</span></span>| <span data-ttu-id="44084-125">Terceiro atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="44084-125">Third customizable extension attribute.</span></span> |
|<span data-ttu-id="44084-126">extensionAttribute4</span><span class="sxs-lookup"><span data-stu-id="44084-126">extensionAttribute4</span></span>|<span data-ttu-id="44084-127">String</span><span class="sxs-lookup"><span data-stu-id="44084-127">String</span></span>| <span data-ttu-id="44084-128">Quarto atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="44084-128">Fourth customizable extension attribute.</span></span> |
|<span data-ttu-id="44084-129">extensionAttribute5</span><span class="sxs-lookup"><span data-stu-id="44084-129">extensionAttribute5</span></span>|<span data-ttu-id="44084-130">String</span><span class="sxs-lookup"><span data-stu-id="44084-130">String</span></span>| <span data-ttu-id="44084-131">Quinto atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="44084-131">Fifth customizable extension attribute.</span></span> |
|<span data-ttu-id="44084-132">extensionAttribute6</span><span class="sxs-lookup"><span data-stu-id="44084-132">extensionAttribute6</span></span>|<span data-ttu-id="44084-133">String</span><span class="sxs-lookup"><span data-stu-id="44084-133">String</span></span>| <span data-ttu-id="44084-134">Sexto atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="44084-134">Sixth customizable extension attribute.</span></span> |
|<span data-ttu-id="44084-135">extensionAttribute7</span><span class="sxs-lookup"><span data-stu-id="44084-135">extensionAttribute7</span></span>|<span data-ttu-id="44084-136">String</span><span class="sxs-lookup"><span data-stu-id="44084-136">String</span></span>| <span data-ttu-id="44084-137">Sétimo atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="44084-137">Seventh customizable extension attribute.</span></span> |
|<span data-ttu-id="44084-138">extensionAttribute8</span><span class="sxs-lookup"><span data-stu-id="44084-138">extensionAttribute8</span></span>|<span data-ttu-id="44084-139">String</span><span class="sxs-lookup"><span data-stu-id="44084-139">String</span></span>| <span data-ttu-id="44084-140">Oitavo atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="44084-140">Eighth customizable extension attribute.</span></span> |
|<span data-ttu-id="44084-141">extensionAttribute9</span><span class="sxs-lookup"><span data-stu-id="44084-141">extensionAttribute9</span></span>|<span data-ttu-id="44084-142">String</span><span class="sxs-lookup"><span data-stu-id="44084-142">String</span></span>| <span data-ttu-id="44084-143">Nono atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="44084-143">Ninth customizable extension attribute.</span></span> |
|<span data-ttu-id="44084-144">extensionAttribute10</span><span class="sxs-lookup"><span data-stu-id="44084-144">extensionAttribute10</span></span>|<span data-ttu-id="44084-145">String</span><span class="sxs-lookup"><span data-stu-id="44084-145">String</span></span>| <span data-ttu-id="44084-146">Décimo atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="44084-146">Tenth customizable extension attribute.</span></span> |
|<span data-ttu-id="44084-147">extensionAttribute11</span><span class="sxs-lookup"><span data-stu-id="44084-147">extensionAttribute11</span></span>|<span data-ttu-id="44084-148">String</span><span class="sxs-lookup"><span data-stu-id="44084-148">String</span></span>| <span data-ttu-id="44084-149">Décimo primeiro atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="44084-149">Eleventh customizable extension attribute.</span></span> |
|<span data-ttu-id="44084-150">extensionAttribute12</span><span class="sxs-lookup"><span data-stu-id="44084-150">extensionAttribute12</span></span>|<span data-ttu-id="44084-151">String</span><span class="sxs-lookup"><span data-stu-id="44084-151">String</span></span>| <span data-ttu-id="44084-152">Décimo segundo atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="44084-152">Twelfth customizable extension attribute.</span></span> |
|<span data-ttu-id="44084-153">extensionAttribute13</span><span class="sxs-lookup"><span data-stu-id="44084-153">extensionAttribute13</span></span>|<span data-ttu-id="44084-154">String</span><span class="sxs-lookup"><span data-stu-id="44084-154">String</span></span>| <span data-ttu-id="44084-155">Décimo terceiro atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="44084-155">Thirteenth customizable extension attribute.</span></span> |
|<span data-ttu-id="44084-156">extensionAttribute14</span><span class="sxs-lookup"><span data-stu-id="44084-156">extensionAttribute14</span></span>|<span data-ttu-id="44084-157">String</span><span class="sxs-lookup"><span data-stu-id="44084-157">String</span></span>| <span data-ttu-id="44084-158">Décimo quarto atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="44084-158">Fourteenth customizable extension attribute.</span></span> |
|<span data-ttu-id="44084-159">extensionAttribute15</span><span class="sxs-lookup"><span data-stu-id="44084-159">extensionAttribute15</span></span>|<span data-ttu-id="44084-160">String</span><span class="sxs-lookup"><span data-stu-id="44084-160">String</span></span>| <span data-ttu-id="44084-161">Décimo quinto atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="44084-161">Fifteenth customizable extension attribute.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="44084-162">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="44084-162">JSON representation</span></span>

<span data-ttu-id="44084-163">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="44084-163">Here is a JSON representation of the resource</span></span>

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

