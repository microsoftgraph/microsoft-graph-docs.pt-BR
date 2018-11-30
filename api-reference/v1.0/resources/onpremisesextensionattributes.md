---
title: tipo de recurso de onPremisesExtensionAttributes
description: A propriedade **onPremisesExtensionAttributes** da entidade do usuário contém quinze propriedades de atributo de extensão personalizada. Um usuário **onPremisesSyncEnabled** , esse conjunto de propriedades é administrado no Active Directory no local e sincronizado com o Azure AD e é somente leitura. Para um usuário somente na nuvem (onde **onPremisesSyncEnabled** é false), essas propriedades podem ser definida durante a criação ou atualização.
ms.openlocfilehash: e5a56b5a846cf48cfc819b6d884689be10d6992e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27005670"
---
# <a name="onpremisesextensionattributes-resource-type"></a><span data-ttu-id="3c6a6-105">tipo de recurso de onPremisesExtensionAttributes</span><span class="sxs-lookup"><span data-stu-id="3c6a6-105">onPremisesExtensionAttributes resource type</span></span>

<span data-ttu-id="3c6a6-106">A propriedade **onPremisesExtensionAttributes** da entidade do [usuário](user.md) contém quinze propriedades de atributo de extensão personalizada.</span><span class="sxs-lookup"><span data-stu-id="3c6a6-106">The **onPremisesExtensionAttributes** property of the [user](user.md) entity contains fifteen custom extension attribute properties.</span></span> <span data-ttu-id="3c6a6-107">Um usuário **onPremisesSyncEnabled** , esse conjunto de propriedades é administrado no Active Directory no local e sincronizado com o Azure AD e é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3c6a6-107">For an **onPremisesSyncEnabled** user, this set of properties is mastered in on-premises Active Directory and synchronized to Azure AD, and is read-only.</span></span> <span data-ttu-id="3c6a6-108">Para um usuário somente na nuvem (onde **onPremisesSyncEnabled** é false), essas propriedades podem ser definida durante a criação ou atualização.</span><span class="sxs-lookup"><span data-stu-id="3c6a6-108">For a cloud-only user (where **onPremisesSyncEnabled** is false), these properties may be set during creation or update.</span></span>


## <a name="properties"></a><span data-ttu-id="3c6a6-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3c6a6-109">Properties</span></span>
| <span data-ttu-id="3c6a6-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3c6a6-110">Property</span></span>     | <span data-ttu-id="3c6a6-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="3c6a6-111">Type</span></span>   |<span data-ttu-id="3c6a6-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="3c6a6-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3c6a6-113">extensionAttribute1</span><span class="sxs-lookup"><span data-stu-id="3c6a6-113">extensionAttribute1</span></span>|<span data-ttu-id="3c6a6-114">String</span><span class="sxs-lookup"><span data-stu-id="3c6a6-114">String</span></span>| <span data-ttu-id="3c6a6-115">Primeiro atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="3c6a6-115">First customizable extension attribute.</span></span> |
|<span data-ttu-id="3c6a6-116">extensionAttribute2</span><span class="sxs-lookup"><span data-stu-id="3c6a6-116">extensionAttribute2</span></span>|<span data-ttu-id="3c6a6-117">String</span><span class="sxs-lookup"><span data-stu-id="3c6a6-117">String</span></span>| <span data-ttu-id="3c6a6-118">Segundo atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="3c6a6-118">Second customizable extension attribute.</span></span> |
|<span data-ttu-id="3c6a6-119">extensionAttribute3</span><span class="sxs-lookup"><span data-stu-id="3c6a6-119">extensionAttribute3</span></span>|<span data-ttu-id="3c6a6-120">String</span><span class="sxs-lookup"><span data-stu-id="3c6a6-120">String</span></span>| <span data-ttu-id="3c6a6-121">Atributo do terceiro extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="3c6a6-121">Third customizable extension attribute.</span></span> |
|<span data-ttu-id="3c6a6-122">extensionAttribute4</span><span class="sxs-lookup"><span data-stu-id="3c6a6-122">extensionAttribute4</span></span>|<span data-ttu-id="3c6a6-123">String</span><span class="sxs-lookup"><span data-stu-id="3c6a6-123">String</span></span>| <span data-ttu-id="3c6a6-124">Quarto atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="3c6a6-124">Fourth customizable extension attribute.</span></span> |
|<span data-ttu-id="3c6a6-125">extensionAttribute5</span><span class="sxs-lookup"><span data-stu-id="3c6a6-125">extensionAttribute5</span></span>|<span data-ttu-id="3c6a6-126">String</span><span class="sxs-lookup"><span data-stu-id="3c6a6-126">String</span></span>| <span data-ttu-id="3c6a6-127">Atributo do quinto extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="3c6a6-127">Fifth customizable extension attribute.</span></span> |
|<span data-ttu-id="3c6a6-128">extensionAttribute6</span><span class="sxs-lookup"><span data-stu-id="3c6a6-128">extensionAttribute6</span></span>|<span data-ttu-id="3c6a6-129">String</span><span class="sxs-lookup"><span data-stu-id="3c6a6-129">String</span></span>| <span data-ttu-id="3c6a6-130">Sexto atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="3c6a6-130">Sixth customizable extension attribute.</span></span> |
|<span data-ttu-id="3c6a6-131">extensionAttribute7</span><span class="sxs-lookup"><span data-stu-id="3c6a6-131">extensionAttribute7</span></span>|<span data-ttu-id="3c6a6-132">String</span><span class="sxs-lookup"><span data-stu-id="3c6a6-132">String</span></span>| <span data-ttu-id="3c6a6-133">Sétimo atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="3c6a6-133">Seventh customizable extension attribute.</span></span> |
|<span data-ttu-id="3c6a6-134">extensionAttribute8</span><span class="sxs-lookup"><span data-stu-id="3c6a6-134">extensionAttribute8</span></span>|<span data-ttu-id="3c6a6-135">String</span><span class="sxs-lookup"><span data-stu-id="3c6a6-135">String</span></span>| <span data-ttu-id="3c6a6-136">Oitavo atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="3c6a6-136">Eighth customizable extension attribute.</span></span> |
|<span data-ttu-id="3c6a6-137">extensionAttribute9</span><span class="sxs-lookup"><span data-stu-id="3c6a6-137">extensionAttribute9</span></span>|<span data-ttu-id="3c6a6-138">String</span><span class="sxs-lookup"><span data-stu-id="3c6a6-138">String</span></span>| <span data-ttu-id="3c6a6-139">Nono atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="3c6a6-139">Ninth customizable extension attribute.</span></span> |
|<span data-ttu-id="3c6a6-140">extensionAttribute10</span><span class="sxs-lookup"><span data-stu-id="3c6a6-140">extensionAttribute10</span></span>|<span data-ttu-id="3c6a6-141">String</span><span class="sxs-lookup"><span data-stu-id="3c6a6-141">String</span></span>| <span data-ttu-id="3c6a6-142">Décimo atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="3c6a6-142">Tenth customizable extension attribute.</span></span> |
|<span data-ttu-id="3c6a6-143">extensionAttribute11</span><span class="sxs-lookup"><span data-stu-id="3c6a6-143">extensionAttribute11</span></span>|<span data-ttu-id="3c6a6-144">String</span><span class="sxs-lookup"><span data-stu-id="3c6a6-144">String</span></span>| <span data-ttu-id="3c6a6-145">Atributo de extensão Décima primeira personalizável.</span><span class="sxs-lookup"><span data-stu-id="3c6a6-145">Eleventh customizable extension attribute.</span></span> |
|<span data-ttu-id="3c6a6-146">extensionAttribute12</span><span class="sxs-lookup"><span data-stu-id="3c6a6-146">extensionAttribute12</span></span>|<span data-ttu-id="3c6a6-147">String</span><span class="sxs-lookup"><span data-stu-id="3c6a6-147">String</span></span>| <span data-ttu-id="3c6a6-148">Atributo de extensão Décima segunda personalizável.</span><span class="sxs-lookup"><span data-stu-id="3c6a6-148">Twelfth customizable extension attribute.</span></span> |
|<span data-ttu-id="3c6a6-149">extensionAttribute13</span><span class="sxs-lookup"><span data-stu-id="3c6a6-149">extensionAttribute13</span></span>|<span data-ttu-id="3c6a6-150">String</span><span class="sxs-lookup"><span data-stu-id="3c6a6-150">String</span></span>| <span data-ttu-id="3c6a6-151">Atributo de extensão Décima terceira personalizável.</span><span class="sxs-lookup"><span data-stu-id="3c6a6-151">Thirteenth customizable extension attribute.</span></span> |
|<span data-ttu-id="3c6a6-152">extensionAttribute14</span><span class="sxs-lookup"><span data-stu-id="3c6a6-152">extensionAttribute14</span></span>|<span data-ttu-id="3c6a6-153">String</span><span class="sxs-lookup"><span data-stu-id="3c6a6-153">String</span></span>| <span data-ttu-id="3c6a6-154">Atributo de extensão décima quarta personalizável.</span><span class="sxs-lookup"><span data-stu-id="3c6a6-154">Fourteenth customizable extension attribute.</span></span> |
|<span data-ttu-id="3c6a6-155">extensionAttribute15</span><span class="sxs-lookup"><span data-stu-id="3c6a6-155">extensionAttribute15</span></span>|<span data-ttu-id="3c6a6-156">String</span><span class="sxs-lookup"><span data-stu-id="3c6a6-156">String</span></span>| <span data-ttu-id="3c6a6-157">Atributo de extensão Décima quinta personalizável.</span><span class="sxs-lookup"><span data-stu-id="3c6a6-157">Fifteenth customizable extension attribute.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="3c6a6-158">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3c6a6-158">JSON representation</span></span>

<span data-ttu-id="3c6a6-159">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="3c6a6-159">Here is a JSON representation of the resource</span></span>

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