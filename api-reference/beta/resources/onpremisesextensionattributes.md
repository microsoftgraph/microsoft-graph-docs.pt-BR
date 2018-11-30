---
title: tipo de recurso de onPremisesExtensionAttributes
description: A propriedade **onPremisesExtensionAttributes** da entidade do usuário contém quinze propriedades de atributo de extensão personalizada. Um usuário **onPremisesSyncEnabled** , esse conjunto de propriedades é administrado no Active Directory no local e sincronizado com o Azure AD e é somente leitura. Para um usuário somente na nuvem (onde **onPremisesSyncEnabled** é false), essas propriedades podem ser definida durante a criação ou atualização.
ms.openlocfilehash: 547fc8ac19059611f5983a8b5ee0bd905f130f79
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27038633"
---
# <a name="onpremisesextensionattributes-resource-type"></a><span data-ttu-id="e68e9-105">tipo de recurso de onPremisesExtensionAttributes</span><span class="sxs-lookup"><span data-stu-id="e68e9-105">onPremisesExtensionAttributes resource type</span></span>

> <span data-ttu-id="e68e9-106">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="e68e9-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e68e9-107">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="e68e9-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e68e9-108">A propriedade **onPremisesExtensionAttributes** da entidade do [usuário](user.md) contém quinze propriedades de atributo de extensão personalizada.</span><span class="sxs-lookup"><span data-stu-id="e68e9-108">The **onPremisesExtensionAttributes** property of the [user](user.md) entity contains fifteen custom extension attribute properties.</span></span> <span data-ttu-id="e68e9-109">Um usuário **onPremisesSyncEnabled** , esse conjunto de propriedades é administrado no Active Directory no local e sincronizado com o Azure AD e é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e68e9-109">For an **onPremisesSyncEnabled** user, this set of properties is mastered in on-premises Active Directory and synchronized to Azure AD, and is read-only.</span></span> <span data-ttu-id="e68e9-110">Para um usuário somente na nuvem (onde **onPremisesSyncEnabled** é false), essas propriedades podem ser definida durante a criação ou atualização.</span><span class="sxs-lookup"><span data-stu-id="e68e9-110">For a cloud-only user (where **onPremisesSyncEnabled** is false), these properties may be set during creation or update.</span></span>


## <a name="properties"></a><span data-ttu-id="e68e9-111">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e68e9-111">Properties</span></span>
| <span data-ttu-id="e68e9-112">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e68e9-112">Property</span></span>     | <span data-ttu-id="e68e9-113">Tipo</span><span class="sxs-lookup"><span data-stu-id="e68e9-113">Type</span></span>   |<span data-ttu-id="e68e9-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="e68e9-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e68e9-115">extensionAttribute1</span><span class="sxs-lookup"><span data-stu-id="e68e9-115">extensionAttribute1</span></span>|<span data-ttu-id="e68e9-116">String</span><span class="sxs-lookup"><span data-stu-id="e68e9-116">String</span></span>| <span data-ttu-id="e68e9-117">Primeiro atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="e68e9-117">First customizable extension attribute.</span></span> |
|<span data-ttu-id="e68e9-118">extensionAttribute2</span><span class="sxs-lookup"><span data-stu-id="e68e9-118">extensionAttribute2</span></span>|<span data-ttu-id="e68e9-119">String</span><span class="sxs-lookup"><span data-stu-id="e68e9-119">String</span></span>| <span data-ttu-id="e68e9-120">Segundo atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="e68e9-120">Second customizable extension attribute.</span></span> |
|<span data-ttu-id="e68e9-121">extensionAttribute3</span><span class="sxs-lookup"><span data-stu-id="e68e9-121">extensionAttribute3</span></span>|<span data-ttu-id="e68e9-122">String</span><span class="sxs-lookup"><span data-stu-id="e68e9-122">String</span></span>| <span data-ttu-id="e68e9-123">Atributo do terceiro extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="e68e9-123">Third customizable extension attribute.</span></span> |
|<span data-ttu-id="e68e9-124">extensionAttribute4</span><span class="sxs-lookup"><span data-stu-id="e68e9-124">extensionAttribute4</span></span>|<span data-ttu-id="e68e9-125">String</span><span class="sxs-lookup"><span data-stu-id="e68e9-125">String</span></span>| <span data-ttu-id="e68e9-126">Quarto atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="e68e9-126">Fourth customizable extension attribute.</span></span> |
|<span data-ttu-id="e68e9-127">extensionAttribute5</span><span class="sxs-lookup"><span data-stu-id="e68e9-127">extensionAttribute5</span></span>|<span data-ttu-id="e68e9-128">String</span><span class="sxs-lookup"><span data-stu-id="e68e9-128">String</span></span>| <span data-ttu-id="e68e9-129">Atributo do quinto extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="e68e9-129">Fifth customizable extension attribute.</span></span> |
|<span data-ttu-id="e68e9-130">extensionAttribute6</span><span class="sxs-lookup"><span data-stu-id="e68e9-130">extensionAttribute6</span></span>|<span data-ttu-id="e68e9-131">String</span><span class="sxs-lookup"><span data-stu-id="e68e9-131">String</span></span>| <span data-ttu-id="e68e9-132">Sexto atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="e68e9-132">Sixth customizable extension attribute.</span></span> |
|<span data-ttu-id="e68e9-133">extensionAttribute7</span><span class="sxs-lookup"><span data-stu-id="e68e9-133">extensionAttribute7</span></span>|<span data-ttu-id="e68e9-134">String</span><span class="sxs-lookup"><span data-stu-id="e68e9-134">String</span></span>| <span data-ttu-id="e68e9-135">Sétimo atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="e68e9-135">Seventh customizable extension attribute.</span></span> |
|<span data-ttu-id="e68e9-136">extensionAttribute8</span><span class="sxs-lookup"><span data-stu-id="e68e9-136">extensionAttribute8</span></span>|<span data-ttu-id="e68e9-137">String</span><span class="sxs-lookup"><span data-stu-id="e68e9-137">String</span></span>| <span data-ttu-id="e68e9-138">Oitavo atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="e68e9-138">Eighth customizable extension attribute.</span></span> |
|<span data-ttu-id="e68e9-139">extensionAttribute9</span><span class="sxs-lookup"><span data-stu-id="e68e9-139">extensionAttribute9</span></span>|<span data-ttu-id="e68e9-140">String</span><span class="sxs-lookup"><span data-stu-id="e68e9-140">String</span></span>| <span data-ttu-id="e68e9-141">Nono atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="e68e9-141">Ninth customizable extension attribute.</span></span> |
|<span data-ttu-id="e68e9-142">extensionAttribute10</span><span class="sxs-lookup"><span data-stu-id="e68e9-142">extensionAttribute10</span></span>|<span data-ttu-id="e68e9-143">String</span><span class="sxs-lookup"><span data-stu-id="e68e9-143">String</span></span>| <span data-ttu-id="e68e9-144">Décimo atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="e68e9-144">Tenth customizable extension attribute.</span></span> |
|<span data-ttu-id="e68e9-145">extensionAttribute11</span><span class="sxs-lookup"><span data-stu-id="e68e9-145">extensionAttribute11</span></span>|<span data-ttu-id="e68e9-146">String</span><span class="sxs-lookup"><span data-stu-id="e68e9-146">String</span></span>| <span data-ttu-id="e68e9-147">Atributo de extensão Décima primeira personalizável.</span><span class="sxs-lookup"><span data-stu-id="e68e9-147">Eleventh customizable extension attribute.</span></span> |
|<span data-ttu-id="e68e9-148">extensionAttribute12</span><span class="sxs-lookup"><span data-stu-id="e68e9-148">extensionAttribute12</span></span>|<span data-ttu-id="e68e9-149">String</span><span class="sxs-lookup"><span data-stu-id="e68e9-149">String</span></span>| <span data-ttu-id="e68e9-150">Atributo de extensão Décima segunda personalizável.</span><span class="sxs-lookup"><span data-stu-id="e68e9-150">Twelfth customizable extension attribute.</span></span> |
|<span data-ttu-id="e68e9-151">extensionAttribute13</span><span class="sxs-lookup"><span data-stu-id="e68e9-151">extensionAttribute13</span></span>|<span data-ttu-id="e68e9-152">String</span><span class="sxs-lookup"><span data-stu-id="e68e9-152">String</span></span>| <span data-ttu-id="e68e9-153">Atributo de extensão Décima terceira personalizável.</span><span class="sxs-lookup"><span data-stu-id="e68e9-153">Thirteenth customizable extension attribute.</span></span> |
|<span data-ttu-id="e68e9-154">extensionAttribute14</span><span class="sxs-lookup"><span data-stu-id="e68e9-154">extensionAttribute14</span></span>|<span data-ttu-id="e68e9-155">String</span><span class="sxs-lookup"><span data-stu-id="e68e9-155">String</span></span>| <span data-ttu-id="e68e9-156">Atributo de extensão décima quarta personalizável.</span><span class="sxs-lookup"><span data-stu-id="e68e9-156">Fourteenth customizable extension attribute.</span></span> |
|<span data-ttu-id="e68e9-157">extensionAttribute15</span><span class="sxs-lookup"><span data-stu-id="e68e9-157">extensionAttribute15</span></span>|<span data-ttu-id="e68e9-158">String</span><span class="sxs-lookup"><span data-stu-id="e68e9-158">String</span></span>| <span data-ttu-id="e68e9-159">Atributo de extensão Décima quinta personalizável.</span><span class="sxs-lookup"><span data-stu-id="e68e9-159">Fifteenth customizable extension attribute.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="e68e9-160">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e68e9-160">JSON representation</span></span>

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